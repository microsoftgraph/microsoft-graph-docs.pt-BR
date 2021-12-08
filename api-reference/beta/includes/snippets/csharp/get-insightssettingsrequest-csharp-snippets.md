---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 22b8d503fb080f553439e031617048eb9dcb5c8a
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61343707"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var insightsSettings = await graphClient.Organization["{organization-id}"].Settings.ItemInsights
    .Request()
    .GetAsync();

```