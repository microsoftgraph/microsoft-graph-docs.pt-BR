---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d0ce4ddf012b73c30eb1c80997b8a8897e7a7b90
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315656"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var domains = await graphClient.Directory.FederationConfigurations["{samlOrWsFedExternalDomainFederation-id}"].Domains
    .Request()
    .GetAsync();

```