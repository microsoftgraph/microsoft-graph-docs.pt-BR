---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 029f568395f4db3997956bc93746c39ab5ba7ea2
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34445767"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var synchronizationSchema = await graphClient.ServicePrincipals["{servicePrincipalId}"].Synchronization.Jobs["{jobId}"].Schema
    .Request()
    .Header("Authorization","Bearer {Token}")
    .GetAsync();

```