---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5f8e96145ce7b5648f7a5cb362747c7e8dc37aff
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61346002"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var insightsSettings = await graphClient.Organization["{organization-id}"].Settings.PeopleInsights
    .Request()
    .GetAsync();

```