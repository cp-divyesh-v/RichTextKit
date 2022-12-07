# Release Notes

RichTextKit will use semver after 1.0. 

Until then, features may be deprecated in a minor version and removed in the next minor version.



## 0.2

### ✨ New Features

* `NSImage` `cgImage` and `jpegData` are now public.
* `NSAttributedString` has a new `withBlackText()` extension.
* `NSAttributedString` has a new init extension file.
* `RichTextCoordinator` `cancellables` are now public.
* `RichTextCoordinator` `resetHighlightedRangeAppearance()` is now public.
* `RichTextCoordinator` `text` is now mutable.
* `RichTextDataFormat` has a new vendor-specific data format.
* `RichTextImageAttachment` is now open for inheritance. 
* `String` extensions have been made public.

### 🗑️ Deprecated

* `FontSizePicker` `sizes` has been renamed to `values`.
* `PdfDataWriter` has been renamed to `PdfDataReader`.
* `RichTextAlignmentPicker` `alignments` has been renamed to `values`.
* `RichTextCoordinator` `context` has been renamed to `richTextContext`.
* `RichTextDataWriter` `richTextData(with:)` has been renamed to `richTextData(for:)`.

### 💥 Breaking Changes
  
* `RichTextViewRepresentable` `decrementFontSize` has been renamed to `decrementCurrentFontSize` and has no range parameter.
* `RichTextViewRepresentable` `incrementFontSize` has been renamed to `incrementCurrentFontSize` and has no range parameter.  



## 0.1.2

This is a small bugfix release.

### 🐛 Bugs

* `RichTextCoordinator` now subscribes to image pasting.



## 0.1.1

This is a small bugfix release.

### 🐛 Bugs

* `RichTextAlignmentWriter` now uses safe ranges to avoid occasional crashes.



## 0.1

This is the first beta release of RichTextKit.

The release includes the following.

### ✨ Foundational Types

* `RichTextView` is a replacement for `UITextView` and `NSTextView`.
* `RichTextEditor` is a SwiftUI view that embeds a `RichTextView`.
* `RichTextContext` is used to inspect and interact with a `RichTextEditor`.
* `RichTextCoordinator` is used by a `RichTextEditor` to keep the text view and context in sync.  

### ✨ Feature support

RichTextKit adds extensive support for a bunch of rich text features:

* Alignment
* Attributes
* Colors
* Data
* Export
* Fonts
* Images
* Pasteboard extensions
* Pdf
* Sharing
* Styles
* Views