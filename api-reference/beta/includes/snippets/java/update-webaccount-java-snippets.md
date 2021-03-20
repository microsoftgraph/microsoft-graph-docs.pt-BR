---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1f41224ecee778f41106db17896ce08ce16f95c4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968955"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WebAccount webAccount = new WebAccount();
webAccount.webUrl = "https://github.com/innocenty.popov";

graphClient.me().profile().webAccounts("{id}")
    .buildRequest()
    .patch(webAccount);

```