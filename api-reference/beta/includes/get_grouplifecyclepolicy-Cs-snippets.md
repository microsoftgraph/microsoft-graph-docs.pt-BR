---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f6f98ae7674212968a4a4641388df666fa950dc4
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34467864"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupLifecyclePolicies = await graphClient.GroupLifecyclePolicies
    .Request()
    .GetAsync();

```