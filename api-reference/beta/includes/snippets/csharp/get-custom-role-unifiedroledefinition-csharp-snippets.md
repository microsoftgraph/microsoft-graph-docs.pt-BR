---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 35fd1209ce0bd076109a837976ea3b3d6fd108ec
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/02/2020
ms.locfileid: "47330317"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleDefinition = await graphClient.RoleManagement.Directory.RoleDefinitions["f189965f-f560-4c59-9101-933d4c87a91a"]
    .Request()
    .GetAsync();

```