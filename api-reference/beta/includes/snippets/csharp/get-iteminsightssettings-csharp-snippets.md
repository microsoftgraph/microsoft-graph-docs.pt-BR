---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: af94506f8b4557a5ecaf368b247051f8cbe20b8b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796034"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var itemInsightsSettings = await graphClient.Organization["{organization-id}"].Settings.ItemInsights
    .Request()
    .GetAsync();

```