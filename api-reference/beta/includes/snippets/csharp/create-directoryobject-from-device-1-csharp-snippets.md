---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 21d64a2945b94d34fd1c839afc3c9303f0a5fc985925ea45d5ea21b68e5f0a01
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273556"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "{id}"
};

await graphClient.Devices["{device-id}"].RegisteredOwners.References
    .Request()
    .AddAsync(directoryObject);

```