---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c635cf3df508b100746f079ce1ccd90184e26a44
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "37999462"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var keyId = Guid.Parse("f0b0b335-1d71-4883-8f98-567911bfdca6");

await graphClient.Applications["{id}"]
    .RemovePassword(keyId)
    .Request()
    .PostAsync();

```