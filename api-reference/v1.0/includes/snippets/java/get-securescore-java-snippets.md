---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d502cb895deb63ff4ee631c65ea82b82c9aaa785
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974774"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SecureScore secureScore = graphClient.security().secureScores("{id}")
    .buildRequest()
    .get();

```