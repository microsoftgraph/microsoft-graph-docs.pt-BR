---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 22c6bd21b38952dfd58afeb3c8b08a3ff1f3a068
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/30/2019
ms.locfileid: "35933745"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

boolean all = True;

String clientContext = "clientContext-value";

graphClient.app().calls("{id}")
    .cancelMediaProcessing(clientContext)
    .buildRequest()
    .post();

```