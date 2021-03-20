---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bfb9d37c954f9d2ca74594a3675906e3a797ad49
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974096"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PasswordAuthenticationMethod passwordAuthenticationMethod = graphClient.me().authentication().passwordMethods("{id}")
    .buildRequest()
    .get();

```