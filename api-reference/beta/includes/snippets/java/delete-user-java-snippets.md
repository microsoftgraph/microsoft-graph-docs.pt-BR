---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 50d67566f2afa5d4babb72ce6b5246eefae9dde7fa61c5caa7a426ac0e7e824e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215142"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("ba9a3254-9f18-4209-aeb3-9e42a35b5be4")
    .buildRequest()
    .delete();

```