# Architecture

The workflow treats source collection, interpretation, and durable updates as distinct stages.

## Source branches

Separate branches collect recent application commits, project-memory commits, and relevant work items. Keeping them separate prevents one input from accidentally driving repeated downstream work.

## Normalization and merge

Each source is converted to a small common shape before the branches merge. The merged result is used to build a deterministic digest: a predictable summary of what is relevant before optional AI interpretation.

## Optional structured processing

An OpenAI API step may turn the digest into a constrained summary. It adds interpretation support, not autonomous decision-making.

## Review gate and durable memory

The workflow prepares a candidate update. A human reviews it before durable project memory changes. This preserves the distinction between automatically collected signals and accepted knowledge.
