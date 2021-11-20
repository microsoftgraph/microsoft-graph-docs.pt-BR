---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7647a51d8b8eeea22f057305f4c13dcf39a1690fb86ff0ad7043a23f28920fed
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214128"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{item-id}")
    .unfollow()
    .buildRequest()
    .delete();

```