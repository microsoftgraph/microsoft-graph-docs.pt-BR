---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 18217d41210748a8cc393e35067957f57f16bc8cc98d049302a5e44788f2c6de
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57271946"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var itemInsightsSettings = await graphClient.Organization["{organization-id}"].Settings.ItemInsights
    .Request()
    .GetAsync();

```