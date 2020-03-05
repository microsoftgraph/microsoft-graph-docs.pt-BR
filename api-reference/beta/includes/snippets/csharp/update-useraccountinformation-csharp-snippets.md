---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fde7ad53c5ca7dca91d2c292ceffe5df92d15284
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "37996233"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userAccountInformation = new UserAccountInformation
{
    AgeGroup = "ageGroup-value",
    CountryCode = "countryCode-value",
    PreferredLanguageTag = new LocaleInfo
    {
        Locale = "locale-value",
        DisplayName = "displayName-value"
    },
    UserPrincipalName = "userPrincipalName-value"
};

await graphClient.Me.Profile.Account["{id}"]
    .Request()
    .UpdateAsync(userAccountInformation);

```