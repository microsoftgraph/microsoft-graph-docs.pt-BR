---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cb7466344ee4e4fa46366f8eb8f6dfe6a9061488
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865724"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var clientContext = "clientContext-value";

await graphClient.Communications.Calls["57dab8b1-894c-409a-b240-bd8beae78896"]
    .Mute(clientContext)
    .Request()
    .PostAsync();

```