---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cc85dc86495939a15b11fbdc37bf5494aae16ce3cf82c633e1552717d89d65b9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327668"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contactFolder = new ContactFolder
{
    ParentFolderId = "parentFolderId-value",
    DisplayName = "displayName-value"
};

await graphClient.Me.ContactFolders["{contactFolder-id}"]
    .Request()
    .UpdateAsync(contactFolder);

```