---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 876649c8d09edfdc494789d927c71a131577dbbefbd9c5698c9af1ecadd20d20
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898208"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().pendingAccessReviewInstances("70a68410-67f3-4d4c-b946-6989e050be19")
    .acceptRecommendations()
    .buildRequest()
    .post();

```