---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 35be88081facab04672059b08f76843986caaf9e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982475"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrinterShare printerShare = new PrinterShare();
printerShare.displayName = "ShareName";
printerShare.allowAllUsers = false;
printerShare.additionalDataManager().put("printer@odata.bind", new JsonPrimitive("https://graph.microsoft.com/v1.0/print/printers/{printerId}"));

graphClient.print().shares()
    .buildRequest()
    .post(printerShare);

```