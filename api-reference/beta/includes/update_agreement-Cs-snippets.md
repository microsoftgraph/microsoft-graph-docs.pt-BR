---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 667322331d4082546634e12b8187ceb2e1efbb4e
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34465689"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var agreement = new Agreement
{
    DisplayName = "displayName-value",
    IsViewingBeforeAcceptanceRequired = true
};

await graphClient.Agreements["'id'"]
    .Request()
    .UpdateAsync(agreement);

```