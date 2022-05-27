---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aa217ee6aa8b25b18aa09e42212b4319f50babfc036401aefafca2f678c5209a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100170"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identity().b2cUserFlows("B2C_1_CustomerSignUp").identityProviders("Facebook-OAUTH").reference()
    .buildRequest()
    .delete();

```