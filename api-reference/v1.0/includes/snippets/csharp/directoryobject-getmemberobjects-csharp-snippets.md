---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dceb7ffd8f9d292300a527ec962ac1f9668d884d2a657b99f1ae327b165207b4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273133"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityEnabledOnly = true;

await graphClient.DirectoryObjects["{directoryObject-id}"]
    .GetMemberObjects(securityEnabledOnly)
    .Request()
    .PostAsync();

```