---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 18576a9a026d9dbff4c09fde918839481db3ebc7
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34474440"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var children = await graphClient.Me.Drive.Items["{item-id}"].Children
    .Request()
    .Expand("thumbnails")
    .GetAsync();

```