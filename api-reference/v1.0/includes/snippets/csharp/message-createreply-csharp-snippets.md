---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2acaaf13bac2dbb12e11e527259e6114c7f7201b
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "37428758"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Messages["{id}"]
    .CreateReply(null,null)
    .Request()
    .PostAsync();

```