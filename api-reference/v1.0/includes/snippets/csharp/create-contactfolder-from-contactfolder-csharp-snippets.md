---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fc4c5a7941972265fe867dd36b32d3cbb6a2bbbb
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507588"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contactFolder = new ContactFolder
{
    DisplayName = "Family"
};

await graphClient.Me.ContactFolders["{contactFolder-id}"].ChildFolders
    .Request()
    .AddAsync(contactFolder);

```