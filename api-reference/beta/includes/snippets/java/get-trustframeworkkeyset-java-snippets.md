---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 747cd7bdd0c4200a08adacb7342a3fe6b05e25cd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982165"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TrustFrameworkKeySet trustFrameworkKeySet = graphClient.trustFramework().keySets("{id}")
    .buildRequest()
    .get();

```