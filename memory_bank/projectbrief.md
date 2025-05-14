# DevLedger Project Brief

## Project Overview
DevLedger is a Python library that transforms code comments into a queryable, evolving knowledge graph across hardware and firmware domains through pattern-based tracking and LLM-powered analysis.

## Core Requirements

### 1. Comment Management
- Pattern-based comment tracking system
- Multi-level comment organization (Information/Debug/Technical)
- Support for multiple programming languages
- Git integration for comment persistence

### 2. Knowledge Storage
- Structured storage in `.devl` directory
- JSON/YAML-based comment storage
- Vector database integration for semantic search
- Git object model integration

### 3. Intelligence Layer
- LLM integration for analysis and queries
- Pattern recognition for comment tracking
- Support for both local and cloud-based models
- Flexible model configuration

### 4. User Interface
- Command-line interface (CLI)
- Git hook integration
- Direct file editing support
- Natural language querying

## Success Criteria
1. Minimal friction in developer workflow
2. Reliable comment tracking through code changes
3. Effective knowledge preservation and retrieval
4. Cross-domain knowledge integration
5. Extensible architecture for future enhancements

## Technical Constraints
- Python 3.8+ compatibility
- Git 2.25+ requirement
- Support for local LLM deployment
- Minimal external dependencies for core functionality

## Development Phases
1. Core Comment Tracking (2 months)
2. LLM Integration (2 months)
3. Hardware Integration (2 months)
4. Extended Capabilities (2 months)

## Initial Focus
For the first release (v0.1.0), we will focus on:
1. Basic comment tracking system
2. Simple git hook integration
3. Core CLI functionality
4. Basic LLM integration
5. Essential file storage structure