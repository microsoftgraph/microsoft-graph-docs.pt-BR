---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dcbf4711bff496a2b5bfcc76528b5671840ca3a4570586c5ed278467a9eaa274
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214781"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

User user = new User();
user.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/users/{id}"));

graphClient.print().shares("{id}").allowedUsers().references()
    .buildRequest()
    .post(user);

```