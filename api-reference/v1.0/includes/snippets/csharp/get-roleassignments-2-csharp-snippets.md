---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c7b31dcd3b7af292141c88fe2437ed31bdf9b632
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59130402"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleAssignments = await graphClient.RoleManagement.Directory.RoleAssignments
    .Request()
    .Filter(" principalId eq 'f1847572-48aa-47aa-96a3-2ec61904f41f'")
    .GetAsync();

```