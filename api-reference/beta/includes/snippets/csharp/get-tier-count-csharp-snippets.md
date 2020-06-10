---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eb368dc1d71959e0556e2d9ea63330c6729ee8c9
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684548"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = await graphClient.Users["{id}"].TransitiveMemberOf
    .Request()
    .Header("ConsistencyLevel","eventual")
    .Search("displayName:tier")
    .Select("displayName,id")
    .OrderBy("displayName ")
    .GetAsync();

```