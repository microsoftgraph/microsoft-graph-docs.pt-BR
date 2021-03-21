---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0c8a336c9ecc1cfada29f867de10657268390527
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969098"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Drive drive = graphClient.users("{idOrUserPrincipalName}").drive()
    .buildRequest()
    .get();

```