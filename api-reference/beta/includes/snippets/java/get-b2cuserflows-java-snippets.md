---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f3c4f92f2099d4d1e6613a9a3d634d917d1ab564
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977492"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

B2cIdentityUserFlow b2cIdentityUserFlow = graphClient.identity().b2cUserFlows("{id}")
    .buildRequest()
    .get();

```