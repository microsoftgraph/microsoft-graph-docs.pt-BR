---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 369234082a2579d848232015efe304d92406d7f7
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60689185"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var federatedIdentityCredentials = await graphClient.Applications["{application-id}"].FederatedIdentityCredentials
    .Request()
    .GetAsync();

```