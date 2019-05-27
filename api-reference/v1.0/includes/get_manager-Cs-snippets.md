---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 731d2eed800b134c9ca598be8760f0afbb64c73f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34477786"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = await graphClient.Users["{id|userPrincipalName}"].Manager
    .Request()
    .GetAsync();

```