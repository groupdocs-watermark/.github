<h1 align="center">GroupDocs.Watermark</h1>

<h3 align="center">Document Watermarking API for 40+ Document and Image Formats</h3>

<p align="center">
  <strong>GroupDocs.Watermark</strong> is an on-premise document-watermarking API that adds text and image watermarks to PDF, Word, Excel, PowerPoint, Visio, email and image files - with control over position, size, rotation, opacity, tiling and locking - and searches, edits and removes the watermarks a document already carries, including ones added by other tools. SDKs for .NET, Java, Node.js and Python.
</p>

[![Product Page](https://img.shields.io/badge/Product%20Page-2865E0?style=for-the-badge&logo=appveyor&logoColor=white)](https://products.groupdocs.com/watermark/)
[![Docs](https://img.shields.io/badge/Docs-2865E0?style=for-the-badge&logo=Hugo&logoColor=white)](https://docs.groupdocs.com/watermark/)
[![Demos](https://img.shields.io/badge/Demos-2865E0?style=for-the-badge&logo=appveyor&logoColor=white)](https://products.groupdocs.app/watermark/family)
[![API](https://img.shields.io/badge/API-2865E0?style=for-the-badge&logo=html5&logoColor=white)](https://reference.groupdocs.com/watermark/)
[![Blog](https://img.shields.io/badge/Blog-2865E0?style=for-the-badge&logo=WordPress&logoColor=white)](https://blog.groupdocs.com/category/watermark/)
[![Search](https://img.shields.io/badge/Search-2865E0?style=for-the-badge&logo=searchengin&logoColor=white)](https://search.groupdocs.com/)
[![Support](https://img.shields.io/badge/Support-2865E0?style=for-the-badge&logo=Discourse&logoColor=white)](https://forum.groupdocs.com/c/watermark)
[![Temp License](https://img.shields.io/badge/Temp%20License-2865E0?style=for-the-badge&logo=rocket&logoColor=white)](https://purchase.groupdocs.com/temporary-license)

## Latest Watermark News & Updates
* **NEW:** [GroupDocs.Watermark for Python via .NET 26.10](https://pypi.org/project/groupdocs-watermark-net/) on PyPI: engine 26.9 with the .NET 10 runtime embedded, Python 3.5 - 3.14 on Windows, Linux and macOS (Intel and Apple Silicon), and Python callbacks for page previews and logging. [Release notes](https://releases.groupdocs.com/watermark/python-net/release-notes/).
* Published [GroupDocs.Watermark 26.9](https://www.nuget.org/packages/GroupDocs.Watermark/) for .NET on NuGet: evaluation mode now allows searching, editing and removing watermarks and adding more than one per document, and PDF image-artifact search is fixed.
* Released [GroupDocs.Watermark.Mcp 26.9](https://www.nuget.org/packages/GroupDocs.Watermark.Mcp): an MCP server that lets AI agents add, find and remove watermarks **locally**. [Get started](https://docs.groupdocs.com/watermark/mcp/).

## Supported Platforms & Repository Groups

### .NET Document Watermarking (C#, ASP.NET, WinForms)
Add, search, edit and remove watermarks in PDF, Office, Visio, email and image files on .NET Framework 4.5+ and .NET 6, 8 and 10.
* **[GroupDocs.Watermark-for-.NET](https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-.NET)**: Core API examples for adding, searching and removing watermarks.
* **[Protect Word Documents](https://github.com/groupdocs-watermark/protect-word-documents-using-groupdocs-watermark-dotnet)**: a use-case sample for locked, removal-resistant Word watermarks.

```csharp
using GroupDocs.Watermark;
using GroupDocs.Watermark.Watermarks;

using (var watermarker = new Watermarker("document.pdf"))
{
    var watermark = new TextWatermark("Confidential", new Font("Arial", 36));
    watermark.ForegroundColor = Color.Red;
    watermark.Opacity = 0.5;
    watermarker.Add(watermark);
    watermarker.Save("watermarked.pdf");
}
```

### Java Document Watermarking (Maven, Spring)
Native Java library for watermarking PDF, Office, Visio, email and image files.
* **[GroupDocs.Watermark-for-Java](https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Java)**: Java examples; the package `com.groupdocs:groupdocs-watermark` comes from the [GroupDocs Maven repository](https://releases.groupdocs.com/java/repo/).

```java
import com.groupdocs.watermark.Watermarker;
import com.groupdocs.watermark.watermarks.Color;
import com.groupdocs.watermark.watermarks.Font;
import com.groupdocs.watermark.watermarks.TextWatermark;

// Add a text watermark to a PDF
Watermarker watermarker = new Watermarker("document.pdf");
TextWatermark watermark = new TextWatermark("Confidential", new Font("Arial", 36));
watermark.setForegroundColor(Color.getRed());
watermark.setOpacity(0.5);
watermarker.add(watermark);
watermarker.save("watermarked.pdf");
watermarker.close();
```

### Node.js Document Watermarking (Node.js via Java)
Add watermarking to Node.js services and scripts with the Java engine.
* **[GroupDocs.Watermark-for-Node.js-via-Java](https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Node.js-via-Java)**: Node.js examples; install with `npm install @groupdocs/groupdocs.watermark`.

```javascript
const groupdocs = require('@groupdocs/groupdocs.watermark');

// Add a text watermark to a PDF
const watermarker = new groupdocs.Watermarker('document.pdf');
const watermark = new groupdocs.TextWatermark('Confidential', new groupdocs.Font('Arial', 36));
watermark.setForegroundColor(groupdocs.Color.getRed());
watermark.setOpacity(0.5);
watermarker.add(watermark);
watermarker.save('watermarked.pdf');
watermarker.close();
```

### Python Document Watermarking (Python via .NET)
A self-contained Python package with the .NET runtime embedded: `pip install groupdocs-watermark-net`, Python 3.5 - 3.14.
* **[GroupDocs.Watermark-for-Python-via-.NET](https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Python-via-.NET)**: Runnable examples for every documented scenario, with a Dockerfile.
* [PyPI](https://pypi.org/project/groupdocs-watermark-net/) | [Docs](https://docs.groupdocs.com/watermark/python-net/) | [API Reference](https://reference.groupdocs.com/watermark/python-net/) | [Release Notes](https://releases.groupdocs.com/watermark/python-net/release-notes/)

```python
from groupdocs.watermark import Watermarker
from groupdocs.watermark.watermarks import TextWatermark, Font, Color

with Watermarker("document.pdf") as watermarker:
    watermark = TextWatermark("Confidential", Font("Arial", 36.0))
    watermark.foreground_color = Color.red
    watermark.opacity = 0.5
    watermarker.add(watermark)
    watermarker.save("watermarked.pdf")
```

### MCP Server for AI Agents (Claude, Cursor, Copilot)
Let AI agents watermark documents through the GroupDocs engine, **locally over MCP**: no uploads, works in evaluation mode out of the box and with your existing license.
* **[GroupDocs.Watermark.Mcp](https://github.com/groupdocs-watermark/GroupDocs.Watermark.Mcp)**: The MCP server: add text and image watermarks, search for and remove existing ones, and read document info.
* **[GroupDocs.Mcp.Installer](https://github.com/groupdocs/GroupDocs.Mcp.Installer)**: Cross-platform installer with per-client registration (Claude Desktop, Claude Code, VS Code, Cursor and more).
* **[GroupDocs.Watermark.Mcp.Tests](https://github.com/groupdocs-watermark/GroupDocs.Watermark.Mcp.Tests)**: Integration suite that verifies every published release.

```bash
# Install and run in one command (.NET 10), then ask your agent:
dnx GroupDocs.Watermark.Mcp --yes
```

> "Add a diagonal CONFIDENTIAL watermark to every PDF in my contracts folder."
> "Find the old draft watermarks in report.docx and remove them."

[MCP documentation](https://docs.groupdocs.com/watermark/mcp/) | [NuGet](https://www.nuget.org/packages/GroupDocs.Watermark.Mcp) | [Docker](https://github.com/orgs/groupdocs-watermark/packages/container/package/watermark-net-mcp) | [MCP Registry](https://registry.modelcontextprotocol.io/v0/servers?search=io.github.groupdocs-watermark/groupdocs-watermark-mcp)

## Business Use-Cases
- Stamp "Confidential" or "Draft" across contracts, NDAs and reports before they leave the company.
- Brand outgoing documents with a logo watermark, tiled or placed per page.
- Lock watermarks in Word documents so recipients cannot edit or delete them.
- Find and remove outdated watermarks, including ones added by other tools, in bulk.
- Watermark page previews for document portals and review workflows.

## API Key Features & Benefits
- 40+ formats: PDF, Word (DOC, DOCX, RTF, ODT and templates), Excel (XLS, XLSX and templates), PowerPoint (PPT, PPTX and shows), Visio (VSD, VSDX and more), email (EML, EMLX, MSG, OFT) and images (PNG, JPG, BMP, GIF, TIFF, WEBP, JPEG 2000).
- Text and image watermarks with font, color, opacity, rotation, alignment, margins, sizing and tiling.
- Format-specific placement: PDF artifacts and annotations, slide and worksheet backgrounds, headers and footers, Visio pages, locked Word sections.
- Search watermarks by text, regular expression, image similarity or formatting, then edit or remove them.
- Document info and page previews; password-protected documents.

## Getting Started
- .NET: `dotnet add package GroupDocs.Watermark`
- Java: add `com.groupdocs:groupdocs-watermark` from the GroupDocs repository, `https://releases.groupdocs.com/java/repo/`
- Node.js: `npm install @groupdocs/groupdocs.watermark`
- Python: `pip install groupdocs-watermark-net`
- Run the sample projects from the repositories above to add, search and remove watermarks.

## Technical Support & Resources
- Documentation and tutorials: https://docs.groupdocs.com/watermark/
- Free support forum: https://forum.groupdocs.com/c/watermark
- Temporary license for full-feature evaluation: https://purchase.groupdocs.com/temporary-license

## Tags

`document-watermark` `pdf-watermark` `add-watermark` `remove-watermark` `watermark-search` `content-protection` `watermarking-api` `python` `mcp` `mcp-server` `ai-agents`
