---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5c8a043b3e60740bca3d2b5f858625a6add89077
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969493"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.policies().authenticationMethodsPolicy().authenticationMethodConfigurations("sms")
    .buildRequest()
    .delete();

```