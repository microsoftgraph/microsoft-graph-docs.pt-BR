---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 09b06080ddf34001a165736d9ace4432e1b5777a
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50500507"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personAnnualEvent = new PersonAnnualEvent
{
    AllowedAudiences = AllowedAudiences.Contacts
};

await graphClient.Me.Profile.Anniversaries["{id}"]
    .Request()
    .UpdateAsync(personAnnualEvent);

```