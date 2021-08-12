---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fcec70f75c4fbaaf5d37a698fdd6fdbe7d32226b6568ec41a0585320e27c5ee8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54274965"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintUsageByPrinterCollectionPage monthlyPrintUsageByPrinter = graphClient.print().reports().monthlyPrintUsageByPrinter()
    .buildRequest()
    .get();

```