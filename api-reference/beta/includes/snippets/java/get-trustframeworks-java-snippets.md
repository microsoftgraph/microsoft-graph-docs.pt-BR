---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4b4387e65289d8363bf5418adee00acc81be0f55
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977883"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TrustFrameworkPolicyCollectionPage policies = graphClient.trustFramework().policies()
    .buildRequest()
    .get();

```