---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 273921dab668b5b947287cbbd82e7889da1ddc5c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706112"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var content = await graphClient.Me.Drive.Items["{item-id}"].Thumbnails["{thumb-id}"].{size}.Content
    .Request()
    .GetAsync();

```