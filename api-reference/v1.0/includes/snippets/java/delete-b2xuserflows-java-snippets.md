---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 462fbaef97a74e18df87109e882079776c844ef52c2ec32db809a36471f7b57a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327172"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identity().b2xUserFlows("B2X_1_Partner")
    .buildRequest()
    .delete();

```