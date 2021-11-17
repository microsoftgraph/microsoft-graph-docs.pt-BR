---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1fda3f52161b805692c7d79e58eaea1e3c67060644242a2fe5cc7d87bd912c92
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159888"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().profile().webAccounts("{id}")
    .buildRequest()
    .delete();

```