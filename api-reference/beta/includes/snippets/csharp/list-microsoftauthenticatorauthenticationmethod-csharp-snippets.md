---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 00efa06abd19b51a10ed5d5f9b8f183484b067019c91ba2030b595589c9588e6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57271940"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var microsoftAuthenticatorMethods = await graphClient.Users["{user-id}"].Authentication.MicrosoftAuthenticatorMethods
    .Request()
    .GetAsync();

```