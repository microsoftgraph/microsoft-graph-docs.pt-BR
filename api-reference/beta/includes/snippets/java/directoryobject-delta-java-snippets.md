---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 33598a55c8cd6745ac4bd292fbd54a903635a712
ms.sourcegitcommit: a9731e19589dcb5c0c6fe2e24b008c86573ef803
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "49845921"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObject directoryObject = graphClient.directoryObjects("delta")
    .buildRequest()
    .filter("isOf('Microsoft.Graph.User') or isOf('Microsoft.Graph.Group')")
    .get();

```