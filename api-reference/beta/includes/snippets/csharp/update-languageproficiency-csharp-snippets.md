---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8a72084e2773add15039a45db7606bee8527bd31
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37998239"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var languageProficiency = new LanguageProficiency
{
    DisplayName = "displayName-value",
    Tag = "tag-value",
    Proficiency = LanguageProficiencyLevel.Elementary
};

await graphClient.Me.Profile.Languages["{id}"]
    .Request()
    .UpdateAsync(languageProficiency);

```