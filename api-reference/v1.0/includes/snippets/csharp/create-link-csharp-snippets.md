---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ea6a0dafb64aab774d78c98e4d60e82f3a93894e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35466069"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var type = "view";

var scope = "anonymous";

await graphClient.Me.Drive.Items["{item-id}"]
    .CreateLink(type,scope)
    .Request()
    .PostAsync();

```