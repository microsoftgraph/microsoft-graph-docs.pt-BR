---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 991fc7fdb44c0af9bd4567da5e09e55983deb958
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34450423"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var storageLocation = "storageLocation-value";

await graphClient.Users["{id}"]
    .ExportPersonalData(storageLocation)
    .Request()
    .PostAsync();

```