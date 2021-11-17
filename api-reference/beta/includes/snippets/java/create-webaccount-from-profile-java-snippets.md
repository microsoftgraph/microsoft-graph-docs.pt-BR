---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 21dc1806632a5ecbac86d22e4771092ac290bf561d2fc35c48bb218cbed9dd5c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159635"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WebAccount webAccount = new WebAccount();
webAccount.description = "My Github contributions!";
webAccount.userId = "innocenty.popov";
ServiceInformation service = new ServiceInformation();
service.name = "GitHub";
service.webUrl = "https://github.com";
webAccount.service = service;

graphClient.me().profile().webAccounts()
    .buildRequest()
    .post(webAccount);

```