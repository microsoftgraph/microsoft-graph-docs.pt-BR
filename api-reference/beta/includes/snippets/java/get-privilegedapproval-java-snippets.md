---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eea50ad26b0436a4334aeef3f50466b1ec0684e1
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875934"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPrivilegedApprovalCollectionPage privilegedApproval = graphClient.privilegedApproval()
    .buildRequest()
    .get();

```