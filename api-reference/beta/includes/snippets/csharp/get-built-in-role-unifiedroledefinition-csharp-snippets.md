---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ecb2aeabceece7b26efed369290f4c9adc535e7f
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/02/2020
ms.locfileid: "47330322"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleDefinition = await graphClient.RoleManagement.Directory.RoleDefinitions["fdd7a751-b60b-444a-984c-02652fe8fa1c"]
    .Request()
    .GetAsync();

```