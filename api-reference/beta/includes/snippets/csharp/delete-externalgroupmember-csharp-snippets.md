---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 82ac250794abba2891e41735f1909828b79f29bb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804873"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.External.Connections["{externalConnection-id}"].Groups["{externalGroup-id}"].Members["{externalGroupMember-id}"]
    .Request()
    .DeleteAsync();

```