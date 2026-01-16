# mcp-libre

LibreOffice MCP Server. Provides tools for document operations.

## Requirements

- LibreOffice 24.2+ (command-line access)
- Node.js 18+

## Installation

```bash
npm install
```

## Start

```bash
npm start
```

## Integration with Claude Desktop

Add to `~/.config/claude/claude_desktop_config.json`:

```json
{
  "mcpServers": {
    "mcp-libre": {
      "command": "node",
      "args": ["/path/to/mcp-libre/src/server.js"],
      "env": {}
    }
  }
}
```

## Document Tools

- create_document - Create document
- read_document_text - Extract text
- convert_document - Convert format
- get_document_info - Document metadata
- insert_text_at_position - Insert text
- search_documents - Search by text
- batch_convert_documents - Convert directory
- merge_text_documents - Merge documents
- get_document_statistics - Document statistics

## Section Control Tools

- extract_document_sections - Extract sections by heading level
- replace_document_section - Replace section content
- get_document_structure - Parse document hierarchy
- insert_document_section - Insert section at position
- get_document_outline - Get heading outline
- replace_document_text - Global text replacement

## Spreadsheet Tools

- get_spreadsheet_sheets - List sheet names
- read_spreadsheet_range - Read range with formulas
- read_spreadsheet_data - Read sheet data
- write_spreadsheet_cell - Write cell value
- write_spreadsheet_range - Write range values
- get_sheet_dimensions - Get sheet dimensions

## Resources

- documents - List available documents

## Features

- Section indexing for agentic document access
- Hierarchical document navigation
- Atomic text replacement
- Batch operations
- Format preservation on edits

## License

MIT
