---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 52f42687603248e9444b8534c3de9a7ce1d0e7e5
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44683779"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = await graphClient.Groups["{id}"].Members
    .Request()
    .Header("ConsistencyLevel","eventual")
    .Search("displayName:Pr")
    .Select("displayName,id")
    .OrderBy("displayName ")
    .GetAsync();

```