---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a481897e88af4a73879e2c91f40eab80b89f3a82
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844949"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identity().b2cUserFlows("B2C_1_Customer").languages("es-ES")
    .buildRequest()
    .delete();

```