---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c3bdae788ec1ce77bd9f89aa6819a01f19520d1626e57beb9001bff8487bd250
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273555"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "{id}"
};

await graphClient.Devices["{device-id}"].RegisteredUsers.References
    .Request()
    .AddAsync(directoryObject);

```