---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 78dca39b35a22c530e5860fd0ff6e843de59e301293419a4eb809d01a6fcfec1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899919"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.sites("{sitesId}").permissions("{permissionId}")
    .buildRequest()
    .delete();

```