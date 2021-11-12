---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3371d12061e211bde73cda3727668ccb9ebcf8a76b23dbefb4287fe0f4fe797f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274732"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printUsageByPrinter = await graphClient.Print.Reports.DailyPrintUsageByPrinter["{printUsageByPrinter-id}"]
    .Request()
    .GetAsync();

```