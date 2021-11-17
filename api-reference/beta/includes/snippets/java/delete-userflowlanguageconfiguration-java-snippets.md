---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f6314c6531daaf82cb758ae4959bc86e6c8709d0cb1aa7abbc131cec56f95099
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157700"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identity().b2cUserFlows("B2C_1_Customer").languages("es-ES")
    .buildRequest()
    .delete();

```