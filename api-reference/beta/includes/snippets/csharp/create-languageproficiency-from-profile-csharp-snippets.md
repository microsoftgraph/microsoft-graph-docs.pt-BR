---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 04834a7388229f1d86097b35a08ced50cfb2a400bb58ab411643b7c00661dd86
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216939"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var languageProficiency = new LanguageProficiency
{
    DisplayName = "Norwegian Bokmål",
    Tag = "nb-NO",
    Spoken = LanguageProficiencyLevel.NativeOrBilingual,
    Written = LanguageProficiencyLevel.NativeOrBilingual,
    Reading = LanguageProficiencyLevel.NativeOrBilingual
};

await graphClient.Me.Profile.Languages
    .Request()
    .AddAsync(languageProficiency);

```