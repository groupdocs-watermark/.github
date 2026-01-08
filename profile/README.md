# Document Watermarking API & SDKs

[![Product Page](https://img.shields.io/badge/Product%20Page-2865E0?style=for-the-badge&logo=appveyor&logoColor=white)](https://products.groupdocs.com/watermark/)
[![Docs](https://img.shields.io/badge/Docs-2865E0?style=for-the-badge&logo=Hugo&logoColor=white)](https://docs.groupdocs.com/watermark/)
[![Demos](https://img.shields.io/badge/Demos-2865E0?style=for-the-badge&logo=appveyor&logoColor=white)](https://products.groupdocs.app/watermark/family)
[![API](https://img.shields.io/badge/API-2865E0?style=for-the-badge&logo=html5&logoColor=white)](https://reference.groupdocs.com/watermark/)
[![Blog](https://img.shields.io/badge/Blog-2865E0?style=for-the-badge&logo=WordPress&logoColor=white)](https://blog.groupdocs.com/category/watermark/)
[![Search](https://img.shields.io/badge/Search-2865E0?style=for-the-badge&logo=searchengin&logoColor=white)](https://search.groupdocs.com/)
[![Support](https://img.shields.io/badge/Support-2865E0?style=for-the-badge&logo=Discourse&logoColor=white)](https://forum.groupdocs.com/c/watermark)
[![Temp License](https://img.shields.io/badge/Temp%20License-2865E0?style=for-the-badge&logo=rocket&logoColor=white)](https://purchase.groupdocs.com/temporary-license)

**GroupDocs.Watermark** is an enterprise-grade document watermarking API. Add watermark, create watermark, or remove watermark across PDFs, Word, Excel, PowerPoint, images, Visio, and email with locked, tiled, invisible watermarking for documents and content protection workflows.

## 📰 Latest Watermark News & Updates
* Published [GroupDocs.Watermark 25.11](https://www.nuget.org/packages/GroupDocs.Watermark) — improved invisible watermarking and faster watermark search.
* Introduced new Use-Case to [Secure Word Documents](https://github.com/groupdocs-watermark/protect-word-documents-using-groupdocs-watermark-dotnet)
* New [blog articles](https://blog.groupdocs.com/category/watermark/) on document security and watermark automation for enterprise.

## 📂 Supported Platforms & Repository Groups

### 🌐 .NET Document Watermarking (C#, ASP.NET, WinForms)
High-performance APIs for watermarking documents in .NET Framework and .NET Core.
* **[GroupDocs.Watermark-for-.NET](https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-.NET)**: Core API for adding, removing, and searching watermarks in C# and VB.NET.
* **[Live Demos](https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-.NET/tree/master/Demos/LiveDemos)**: UI examples to protect documents with watermarks.

```csharp
// Quick .NET Watermark Example
using (var watermarker = new Watermarker("source.docx"))
{
    var watermark = new TextWatermark("Confidential", new Font("Arial", 48, FontStyle.Bold));
    watermark.ForegroundColor = Color.DarkGreen;
    watermark.Opacity = 0.5;    
    watermarker.Add(watermark);
    watermarker.Save("result.docx");
}
```

### ☕ Java Document Watermarking (Maven, Spring)
Native Java library for watermarking PDFs, Office documents, images, and more.
* **[GroupDocs.Watermark-for-Java](https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Java)**: Standard Java API for add/remove/search watermark operations.

```java
// Quick Java Watermark Example
try (Watermarker watermarker = new Watermarker("source.pdf")) {
    TextWatermark watermark = new TextWatermark("Draft", new Font("Arial", 36));
    watermark.setOpacity(0.4);
    watermarker.add(watermark);
    watermarker.save("result.pdf");
}
```

### 🟩 Node.js Watermarking (Node.js via Java)
Fast Node.js integration that wraps the Java engine for cross-platform watermark automation.
* **[GroupDocs.Watermark-for-Node.js-via-Java](https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Node.js-via-Java)**: Runnable samples for watermarking Word, PDF, Excel, images, and more from Node.js.

```javascript
// Quick Node.js Watermark Example (path-based)
const groupdocs = require('@groupdocs/groupdocs.watermark');

async function run() {
  const watermarker = new groupdocs.Watermarker('source.docx');
  const watermark = new groupdocs.TextWatermark('Internal Use', new groupdocs.Font('Arial', 42));
  watermark.setOpacity(0.35);
  watermarker.add(watermark);
  await watermarker.save('result.docx');
}

run().catch(console.error);
```

### 🐍 Python Document Watermarking
Python scripts powered by the .NET engine to add or remove watermark content at scale.
* **[GroupDocs.Watermark-for-Python-via-.NET](https://github.com/groupdocs-watermark/GroupDocs.Watermark-for-Python-via-.NET)**: Efficient Python integration for PDF and Word watermarking.

```python
# Quick Python Watermark Example
from groupdocs.watermark import Watermarker
from groupdocs.watermark import TextWatermark, Font

with Watermarker("source.xlsx") as watermarker:
    watermark = TextWatermark("Confidential", Font("Arial", 32))
    watermark.opacity = 0.4
    watermarker.add(watermark)
    watermarker.save("result.xlsx")
```

### Business Use-Cases
Practical watermark workflows teams ship to production:
* **Secure contracts & NDAs:** Tiled “Confidential” stamps plus locked headers for DOCX; see the C# samples in **[Protect Word Documents with GroupDocs.Watermark](https://github.com/groupdocs-watermark/protect-word-documents-using-groupdocs-watermark-dotnet)** for removal-resistant Word protection.
* **Tiled watermarks with templates:** Apply tiled text/image watermarks using presets (spacing, rotation, opacity) to standardize protection across document libraries.
* **Native embedded elements:** Add watermarks as document-native objects (headers, shapes, annotations) to reduce the chance of editing or deletion.

---

## ✅ API Key Features & Benefits
* **Add watermark**: Text, image, logo, and branded custom watermark options.
* **Remove watermark**: Find and delete visible or invisible watermarks in seconds.
* **Invisible watermarking for documents**: Steganographic embedding for tamper-resistant protection.
* **Watermark automation for enterprise**: Batch processing and integration into CI/CD.
* **Content protection with watermarking**: Lock editing, prevent copy/print, preserve metadata.
* **Cross-format support**: PDF, DOCX, XLSX, PPTX, TIFF, PNG, JPG, Visio, EML, MSG, and more.
* **Search & manage**: Detect watermarks by text, color, size, font, or position; accept/reject rules.
* **Performance & scaling**: Optimized for multi-document operations and server-side workloads.

## 🆘 Technical Support & Resources
* **Documentation:** Comprehensive [Guides and Tutorials](https://docs.groupdocs.com/watermark/).
* **Support:** Expert help at the [GroupDocs Free Support Forum](https://forum.groupdocs.com/c/watermark).
* **Evaluation:** Get a [Temporary License](https://purchase.groupdocs.com/temporary-license) for full feature testing.
* **Live Demo:** Try watermarking online at [GroupDocs.Watermark apps](https://products.groupdocs.app/watermark/family).

## 🏷️ Tags

`document-watermark` `pdf-watermark` `add-watermark` `remove-watermark` `invisible-watermarking-for-documents` `content-protection-with-watermarking` `watermark-automation-for-enterprise` `document-security` `custom-watermark` `watermarking-api`
