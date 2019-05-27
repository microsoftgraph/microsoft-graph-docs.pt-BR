---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 93aea26070a6eaa4c1d7e9ed54b32b840339d3f9
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34458145"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = true;

await graphClient.DirectoryObjects["{object-id}"]
    .GetMemberGroups(securityEnabledOnly)
    .Request()
    .PostAsync();

```