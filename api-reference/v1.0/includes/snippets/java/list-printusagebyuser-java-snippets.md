---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 29a84b4f900b7edc3399f73e842574fad9836080
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50768716"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPrintUsageByUserCollectionPage monthlyPrintUsageByUser = graphClient.reports().monthlyPrintUsageByUser()
    .buildRequest()
    .get();

```