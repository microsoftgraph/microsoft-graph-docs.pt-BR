---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5bc726d0b3fe29e3588cdc22b850782537819987
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207152"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var int32 = await graphClient.Groups["{group-id}"].TransitiveMembers.$count
    .Request()
    .Header("ConsistencyLevel","eventual")
    .GetAsync();

```