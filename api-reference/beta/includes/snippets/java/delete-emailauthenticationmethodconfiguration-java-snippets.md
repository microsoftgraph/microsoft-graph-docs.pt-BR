---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e93e47d6b4e7a49d8161c09ca7f41b2c85ae5fc2e54786d48aa954798b959fd3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214766"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().authenticationMethodsPolicy().authenticationMethodConfigurations("email")
    .buildRequest()
    .delete();

```