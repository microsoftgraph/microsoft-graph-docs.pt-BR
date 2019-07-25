---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 18576a9a026d9dbff4c09fde918839481db3ebc7
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35730948"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var children = await graphClient.Me.Drive.Items["{item-id}"].Children
    .Request()
    .Expand("thumbnails")
    .GetAsync();

```