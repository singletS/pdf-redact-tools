# PDF Redact Tools

PDF Redact Tools is a set of tools to help with securely redacting and stripping metadata from documents before publishing.

To use it, convert your original document to a PDF.

Then start by exploding the PDF into PNG files:

    pdf-explode original_document.pdf

This will create a new folder in the same directory as the PDF called (in this case) `original_document_pages`, with a PNG for each page.

Edit each page that needs redacting in graphics editing software like GIMP.

When you're done, combine the PNGs back into a flattened, informationless PDF:

    pdf-merge original_document.pdf

In this case, the final redacted PDF is called `orginal_document-final.pdf`.
