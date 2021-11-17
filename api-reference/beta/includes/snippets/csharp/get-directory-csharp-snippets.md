---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 92a0160fec3b15bf5b5cc82ac16cbda573b0b27eb9da9f5ed370c7ae34adf2d2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217017"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = await graphClient.Directory.DeletedItems["{directoryObject-id}"]
    .Request()
    .GetAsync();

```