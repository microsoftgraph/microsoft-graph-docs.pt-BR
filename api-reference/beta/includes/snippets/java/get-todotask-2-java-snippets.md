---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 909740302a578a224834ec5fc8c7a7fd5f00e2564b9d1447e16ba991d228752d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274712"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TodoTaskCollectionPage tasks = graphClient.me().todo().lists("35e2-35e2-721a-e235-1a72e2351a7").tasks()
    .buildRequest()
    .get();

```