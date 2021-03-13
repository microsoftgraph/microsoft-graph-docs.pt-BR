---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 411236d9cd7956e4e1456effeffc297349b3976e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773092"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LegalHold legalHold = graphClient.compliance().ediscovery().cases("{caseId}").legalHolds("{legalholdId}")
    .buildRequest()
    .get();

```