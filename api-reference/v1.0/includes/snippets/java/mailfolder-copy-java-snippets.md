---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e2efdafe9064bec3d23cd8167ad41936c3739ae3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893260"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String destinationId = "destinationId-value";

graphClient.me().mailFolders("{id}")
    .copy(destinationId)
    .buildRequest()
    .post();

```