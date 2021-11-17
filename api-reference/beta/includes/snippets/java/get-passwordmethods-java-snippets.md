---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9535ebaab5d3935218b59e915d82f2eaf56db11e9c1e19396a23a82f4c391763
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898878"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PasswordAuthenticationMethodCollectionPage passwordMethods = graphClient.me().authentication().passwordMethods()
    .buildRequest()
    .get();

```