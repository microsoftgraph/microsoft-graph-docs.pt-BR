---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 65d71c856d31b94d31a78fcf0ed75afa3c9e69eb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950965"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var emailMethods = await graphClient.Me.Authentication.EmailMethods
    .Request()
    .GetAsync();

```