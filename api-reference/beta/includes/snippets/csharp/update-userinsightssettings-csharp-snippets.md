---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 29f33ba64f0ab5e07ecbbe1efeafe1f63ea955fa1b2a57243462508017d7bbc7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215532"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userInsightsSettings = new UserInsightsSettings
{
    IsEnabled = false
};

await graphClient.Users["{user-id}"].Settings.ItemInsights
    .Request()
    .UpdateAsync(userInsightsSettings);

```