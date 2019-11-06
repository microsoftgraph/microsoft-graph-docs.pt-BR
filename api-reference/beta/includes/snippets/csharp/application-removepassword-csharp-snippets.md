---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c635cf3df508b100746f079ce1ccd90184e26a44
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
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