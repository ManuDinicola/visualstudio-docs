---
title: "Inside the Core Editor | Microsoft Docs"
ms.custom: ""
ms.date: "11/04/2016"
ms.technology: 
  - "vs-ide-sdk"
ms.topic: "conceptual"
helpviewer_keywords: 
  - "editors [Visual Studio SDK], legacy - core editor"
ms.assetid: 8265f31c-c45b-4858-882c-6d9f1e3b9083
author: "gregvanl"
ms.author: "gregvanl"
manager: douge
ms.workload: 
  - "vssdk"
---
# Inside the core editor
The [!INCLUDE[vsprvs](../code-quality/includes/vsprvs_md.md)] core editor is a set of several components that let you modify and query textual information. If you have customized the core editor by using the legacy API, you may continue to use these customizations, which will be routed through editor adapters. It is recommended, however, that you adapt your customizations to the new editor API.  
  
 The following areas are some important aspects of the core editor:  
  
-   Text buffer  
  
-   Text view  
  
-   Code window  
  
-   Text markers  
  
-   Text manager  
  
-   Integration with language services  
  
## In this section  
 [Instantiate the core editor by using the legacy API](../extensibility/instantiating-the-core-editor-by-using-the-legacy-api.md)  
 Provides step-by-step instructions about how to use <xref:Microsoft.VisualStudio.Shell.Interop.IVsEditorFactory.CreateEditorInstance%2A> to create an instance of the core editor.  
  
 [Access the text buffer by using the legacy API](../extensibility/accessing-the-text-buffer-by-using-the-legacy-api.md)  
 Discusses the text buffer's role in the core editor, explains the associated systems that are used to access the buffer, and provides a list of the interfaces implemented by the text buffer object, <xref:Microsoft.VisualStudio.TextManager.Interop.VsTextBuffer>.  
  
 [Text buffer events in the legacy API](../extensibility/text-buffer-events-in-the-legacy-api.md)  
 Provides a list of the interfaces that are used for notification of text buffer events.  
  
 [How to: Register for text buffer events with the legacy API](../extensibility/how-to-register-for-text-buffer-events-with-the-legacy-api.md)  
 Describes how to advise text buffer events.  
  
 [Use the text manager to monitor global settings](../extensibility/using-the-text-manager-to-monitor-global-settings.md)  
 Discusses how the text manager is used to share global preference information with the core editor components and how to receive notification of text manager events.  
  
 [Access theText view by using the legacy API](../extensibility/accessing-thetext-view-by-using-the-legacy-api.md)  
 Describes the text view's role in the core editor and lists the interfaces implemented by the <xref:Microsoft.VisualStudio.TextManager.Interop.VsTextView> object.  
  
 [Customize code windows by using the legacy API](../extensibility/customizing-code-windows-by-using-the-legacy-api.md)  
 Provides information about how a code window is used to enclose the text view, discusses how the code window manager is used to provide decorations to the code window, and provides notification of new views.  
  
 [Change view settings by using the legacy API](../extensibility/changing-view-settings-by-using-the-legacy-api.md)  
 Provides step-by-step instructions about how to force view settings and how to remove forced settings.  
  
 [Language services and the core editor](../extensibility/language-services-and-the-core-editor.md)  
 Describes the instantiation of a language service to control code decorations.  
  
## Related sections  
 [Walkthrough: Create a core editor and registering an editor file type](../extensibility/walkthrough-creating-a-core-editor-and-registering-an-editor-file-type.md)  
 Provides step-by-step instructions about how to start the core editor from managed code.  
  
 [Drop-down bar](../extensibility/drop-down-bar.md)  
 Discusses how the drop-down bar is used in the code window and describes the interfaces that are used when you implement a drop-down bar.  
  
 [Use text markers with the legacy API](../extensibility/using-text-markers-with-the-legacy-api.md)  
 Explains the concept of text markers and how they are used in the core editor, and lists the interfaces that are used to access and manage text markers.  
  
 [How to: Add standard text markers](../extensibility/how-to-add-standard-text-markers.md)  
 Provides step-by-step instructions about how to create a text marker and how to add a custom command to a shortcut menu.  
  
 [How to: Create custom text markers](../extensibility/how-to-create-custom-text-markers.md)  
 Provides step-by-step instructions about how to create a custom text marker and how to provide the marker type as a service.