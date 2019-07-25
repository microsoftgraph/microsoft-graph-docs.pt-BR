---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dee091cb0f94c2ad4228cdd9f7825f6a2eff7778
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878776"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnenoteOperation onenoteOperation = graphClient.me().onenote().operations("{id}")
    .buildRequest()
    .get();

```