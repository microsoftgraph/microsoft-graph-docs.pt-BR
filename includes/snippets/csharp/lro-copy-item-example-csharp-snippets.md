---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bfda972ad2a967a1a147c5aba1cff515ccf32fa9
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48609179"
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