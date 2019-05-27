---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 49b381d367d9a91f62a565247bc865f3785a2304
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34474650"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sharedDriveItem = await graphClient.Shares["{shareIdOrEncodedSharingUrl}"]
    .Request()
    .GetAsync();

```