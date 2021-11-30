---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5db82e141c4a7673a38f66d13825049a153f4677
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61225622"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CustomSecurityAttributeDefinition customSecurityAttributeDefinition = new CustomSecurityAttributeDefinition();
customSecurityAttributeDefinition.status = "Deprecated";

graphClient.directory().customSecurityAttributeDefinitions("Engineering_Project")
    .buildRequest()
    .patch(customSecurityAttributeDefinition);

```