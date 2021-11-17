---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5692e112c7b2b9ec4aac59c2afad1b8ae21b2dbcb74499b39cc8b4d950319fb4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327297"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = graphClient.termStore().groups("1FFD3F87-9464-488A-A0EC-8FB90911182C")
    .buildRequest()
    .get();

```