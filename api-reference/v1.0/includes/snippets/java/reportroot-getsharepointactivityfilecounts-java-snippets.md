---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 861820b852a2f7fc2da3c34a86150463baf93a9c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35893575"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getSharePointActivityFileCounts('D7')
    .buildRequest()
    .get();

```