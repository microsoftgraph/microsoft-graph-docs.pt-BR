---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 74af7cd688d894c294fcfcbaac4998d49377ba2c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35730641"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var Stream = "The contents of the file goes here."

await graphClient.Me.Drive.Items["{item-id}"]
    .Request()
    .PutAsync(Stream);

```