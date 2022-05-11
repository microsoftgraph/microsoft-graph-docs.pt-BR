---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 520d81ba6fa155b01e6efe43dfb92b17bb89561b
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323948"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var organization = await graphClient.Organization["{organization-id}"]
    .Request()
    .GetAsync();

```