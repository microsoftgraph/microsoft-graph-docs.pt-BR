---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 18a08f949873e4f24e78d01d0dbd07cf9aa0e8e6425481296cf382010a15f376
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274761"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var legalHold = new Microsoft.Graph.Ediscovery.LegalHold
{
    Description = "This is a description for a legalHold"
};

await graphClient.Compliance.Ediscovery.Cases["{ediscovery.case-id}"].LegalHolds["{ediscovery.legalHold-id}"]
    .Request()
    .UpdateAsync(legalHold);

```