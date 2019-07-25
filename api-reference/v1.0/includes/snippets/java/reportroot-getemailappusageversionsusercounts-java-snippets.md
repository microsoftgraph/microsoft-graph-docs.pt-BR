---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fabbcfc7fb23b7db0523e5489ea6cb7ca8e0ca0d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35880388"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Report report = graphClient.reports()
    .getEmailAppUsageVersionsUserCounts('D7')
    .buildRequest()
    .get();

```