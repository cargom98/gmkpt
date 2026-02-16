# Product Overview

This is a Kiro Power that integrates Trello project management capabilities into the Kiro IDE. It wraps the Trello MCP server to enable developers to manage Trello boards, lists, cards, and organizations without leaving their development environment.

## Core Functionality

- Board management (list, view details)
- List operations (list, create)
- Card operations (list, create, update, move between lists)
- Organization management (workspaces, boards, team members)

## Authentication

Uses OAuth 1.0a with Trello API. Requires:
- API key from Trello Power-Ups Admin
- Browser-based authorization on first use
- Token cached in `~/.trello_mcp_token.json`

## Target Users

Developers who use Trello for project management and want to integrate task tracking directly into their IDE workflow.
