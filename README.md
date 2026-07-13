# Escalith

**Behavioral Trajectory Analysis for Multi-Turn LLM Safeguards**

Escalith is an AI safety research framework for detecting how misuse risk develops across multi-turn conversations with large language models.

Most safety classifiers evaluate one message at a time. Escalith instead studies the full conversational trajectory, including changes in intent, repeated boundary testing, escalation toward actionable harm, and patterns that may only become visible across several turns.

The project will compare rule-based, single-turn, and conversation-aware detection methods. It will also evaluate false positives and over-refusal using benign conversations involving cybersecurity education, fraud prevention, journalism, research, and fictional writing.

## Research Question

Can a conversation-aware risk model detect emerging misuse earlier than a single-message classifier while preserving legitimate user access?

## Research Objectives

Escalith aims to:

- detect changes in conversational risk over time
- identify the turn where intent becomes clearly actionable
- compare single-turn and conversation-aware classifiers
- measure false positives and safeguard over-refusal
- preserve legitimate educational, research, and creative use
- produce explainable safeguard recommendations
- simulate how detection signals could support real-time safety systems

## Initial Research Scope

The first version will include:

- 200 synthetic multi-turn conversations
- 4 to 6 turns per conversation
- 6 misuse categories
- 3 benign control categories
- turn-level risk labels from 0 to 5
- rule-based and machine-learning baselines
- conversation-aware risk features
- evaluation metrics for precision, recall, F1 score, false-positive rate, and detection delay

## Planned Detection Approaches

1. Rule-based keyword baseline
2. Single-turn text classifier
3. Conversation-aware classifier using prior turns
4. Escalation scoring engine
5. Safeguard intervention policy

## Planned Safeguard Actions

The system will recommend one of the following actions:

- Allow
- Allow with caution
- Ask for clarification
- Send for human review
- Refuse

## Project Status

Escalith is currently in the research design and dataset planning phase.