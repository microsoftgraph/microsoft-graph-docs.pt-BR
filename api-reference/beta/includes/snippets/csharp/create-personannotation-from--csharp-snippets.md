---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2df8b905e5aac8dcae046fb161af198710ee4e9d7cd178c7978a4d1940589976
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275561"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var personAnnotation = new PersonAnnotation
{
    Detail = new ItemBody
    {
        ContentType = BodyType.Text,
        Content = "I am originally from Australia, but grew up in Moscow, Russia."
    },
    DisplayName = "About Me"
};

await graphClient.Me.Profile.Notes
    .Request()
    .AddAsync(personAnnotation);

```