---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 90860b7ca068607a6d0f6f3f3cfaad407dabe462ede485a9de7963dd224e495d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216259"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

WebAccount webAccount = new WebAccount();
webAccount.webUrl = "https://github.com/innocenty.popov";

graphClient.me().profile().webAccounts("{id}")
    .buildRequest()
    .patch(webAccount);

```