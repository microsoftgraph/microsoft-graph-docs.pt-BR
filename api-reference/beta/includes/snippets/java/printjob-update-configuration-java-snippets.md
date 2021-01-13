---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e512616fbf2dc6dcf456c68dd000ba29fc51748d
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49843578"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintJobConfiguration printJobConfiguration = new PrintJobConfiguration();
printJobConfiguration.feedOrientation = PrinterFeedOrientation.LONG_EDGE_FIRST;
LinkedList<IntegerRange> pageRangesList = new LinkedList<IntegerRange>();
IntegerRange pageRanges = new IntegerRange();
pageRanges.start = 1L;
pageRanges.end = 1L;
pageRangesList.add(pageRanges);
printJobConfiguration.pageRanges = pageRangesList;
printJobConfiguration.quality = PrintQuality.MEDIUM;
printJobConfiguration.dpi = 600;
printJobConfiguration.orientation = PrintOrientation.LANDSCAPE;
printJobConfiguration.copies = 1;
printJobConfiguration.duplexMode = PrintDuplexMode.ONE_SIDED;
printJobConfiguration.colorMode = PrintColorMode.BLACK_AND_WHITE;
printJobConfiguration.inputBin = "by-pass-tray";
printJobConfiguration.outputBin = "output-tray";
printJobConfiguration.mediaSize = "A4";
PrintMargin margin = new PrintMargin();
margin.top = 0;
margin.bottom = 0;
margin.left = 0;
margin.right = 0;
printJobConfiguration.margin = margin;
printJobConfiguration.mediaType = "stationery";
printJobConfiguration.finishings = null;
printJobConfiguration.pagesPerSheet = 1;
printJobConfiguration.multipageLayout = PrintMultipageLayout.CLOCKWISE_FROM_BOTTOM_LEFT;
printJobConfiguration.collate = false;
printJobConfiguration.scaling = PrintScaling.SHRINK_TO_FIT;
printJobConfiguration.fitPdfToPage = false;

graphClient.customRequest("/print/printers/d5ef6ec4-07ca-4212-baf9-d45be126bfbb/jobs/44353/configuration", PrintJobConfiguration.class)
    .buildRequest()
    .patch(printJobConfiguration);

```