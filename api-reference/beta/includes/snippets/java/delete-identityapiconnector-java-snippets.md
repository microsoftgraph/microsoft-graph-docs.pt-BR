---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 07d72375ffe72d1e68205e0b08d029458061252b
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49844527"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identity().apiConnectors("{id}")
    .buildRequest()
    .delete();

```