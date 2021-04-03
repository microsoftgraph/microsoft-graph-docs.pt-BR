---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e9f1738fa0985b809f7ca2fce0e01a88192eb996
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51573000"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewInstanceCollectionPage instances = graphClient.identityGovernance().accessReviews().definitions("8564a649-4f67-4e09-88e7-55def6530e88").instances()
    .buildRequest()
    .skip(0)
    .top(100)
    .get();

```