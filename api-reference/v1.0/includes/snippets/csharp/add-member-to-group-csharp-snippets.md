---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dd3e06207a73ee859bbd0bb9a1c73b2d8035fd75
ms.sourcegitcommit: 01f73b4dce6f885da18d62fe800b387c286c7a8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/09/2020
ms.locfileid: "47413320"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "{id}"
};

await graphClient.Groups["{group-id}"].Members.References
    .Request()
    .AddAsync(directoryObject);

```