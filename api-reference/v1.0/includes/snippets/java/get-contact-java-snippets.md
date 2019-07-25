---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1becc7d09e48a29bc42b5d194643734fc072c0b0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885134"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Contact contact = graphClient.me().contacts("{id}")
    .buildRequest()
    .get();

```