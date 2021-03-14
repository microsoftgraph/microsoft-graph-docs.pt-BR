---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bba4d4e58288ac4fe36ec49f02e7c2b535d17aff
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798020"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contact = new Contact
{
    ParentFolderId = "parentFolderId-value",
    Birthday = DateTimeOffset.Parse("datetime-value"),
    FileAs = "fileAs-value",
    DisplayName = "displayName-value",
    GivenName = "givenName-value",
    Initials = "initials-value"
};

await graphClient.Me.ContactFolders["{contactFolder-id}"].Contacts
    .Request()
    .AddAsync(contact);

```