---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c635cf3df508b100746f079ce1ccd90184e26a44
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/15/2019
ms.locfileid: "37994943"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var keyId = Guid.Parse("f0b0b335-1d71-4883-8f98-567911bfdca6");

await graphClient.Applications["{id}"]
    .RemovePassword(keyId)
    .Request()
    .PostAsync();

```