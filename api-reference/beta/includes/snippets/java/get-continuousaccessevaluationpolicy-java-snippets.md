---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 09bdc38e809eea142eb9bd516e7309cd1dd2f0612a9b1a751a4af98c4a6cb6b9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326888"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ContinuousAccessEvaluationPolicy continuousAccessEvaluationPolicy = graphClient.identity().continuousAccessEvaluationPolicy()
    .buildRequest()
    .get();

```