---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b4fd07445e265f38d5de50030ab546caa17b864a
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211885"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AuthenticationContextClassReference authenticationContextClassReference = graphClient.identity().conditionalAccess().authenticationContextClassReferences("c1")
    .buildRequest()
    .get();

```