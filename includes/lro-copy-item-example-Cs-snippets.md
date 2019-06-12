---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bfda972ad2a967a1a147c5aba1cff515ccf32fa9
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34843735"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var parentReference = new ItemReference
{
    Path = "/drive/root:/Documents"
};

var name = "Copy of LargeFolder1";

await graphClient.Me.Drive.Items["{folder-item-id}"]
    .Copy(name,parentReference)
    .Request()
    .PostAsync();

```