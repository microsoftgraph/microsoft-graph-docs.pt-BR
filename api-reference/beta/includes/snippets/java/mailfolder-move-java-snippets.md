---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 52cfb6b3afe425190e4ddd5e573ea02f84a0edd6
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879933"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String destinationId = "destinationId-value";

graphClient.me().mailFolders("{id}")
    .move(destinationId)
    .buildRequest()
    .post();

```