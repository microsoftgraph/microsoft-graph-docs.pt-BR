---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 103b4c2bfaeaef6ce2af5458e9a96a233d546b74
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "37998127"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Profile.Interests["{id}"]
    .Request()
    .DeleteAsync();

```