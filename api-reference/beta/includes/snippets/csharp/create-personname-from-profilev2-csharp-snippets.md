---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c71e8d6e4cf6a7f366754d9bdb6c92469c6de3e4200235a92912e9f59267d8a1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275462"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personName = new PersonName
{
    DisplayName = "Innocenty Popov",
    First = "Innocenty",
    Initials = "IP",
    Last = "Popov",
    LanguageTag = "en-US",
    Maiden = null
};

await graphClient.Me.Profile.Names
    .Request()
    .AddAsync(personName);

```