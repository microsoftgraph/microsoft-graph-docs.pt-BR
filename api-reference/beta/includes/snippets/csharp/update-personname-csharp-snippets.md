---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b692f8afc8e5d840f013b4ddb1abe0845f7620de
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997205"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personName = new PersonName
{
    DisplayName = "displayName-value",
    First = "first-value",
    Initials = "initials-value",
    Last = "last-value",
    LanguageTag = "languageTag-value",
    Maiden = "maiden-value"
};

await graphClient.Me.Profile.Names["{id}"]
    .Request()
    .UpdateAsync(personName);

```