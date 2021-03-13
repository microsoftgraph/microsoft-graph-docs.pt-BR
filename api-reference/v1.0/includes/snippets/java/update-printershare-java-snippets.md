---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f18245f077fe3e60c456851539083113477928ff
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776848"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrinterShare printerShare = new PrinterShare();
printerShare.displayName = "PrinterShare Name";
printerShare.additionalDataManager().put("printer@odata.bind", new JsonPrimitive("https://graph.microsoft.com/v1.0/print/printers/{printerId}"));
printerShare.allowAllUsers = false;

graphClient.print().shares("{printerShareId}")
    .buildRequest()
    .patch(printerShare);

```