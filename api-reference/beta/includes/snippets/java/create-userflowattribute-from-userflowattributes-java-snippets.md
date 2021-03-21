---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f2c0a8804530af1a5d7d16b63cb3b1bfe356556f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50975522"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityUserFlowAttribute identityUserFlowAttribute = new IdentityUserFlowAttribute();
identityUserFlowAttribute.displayName = "Hobby";
identityUserFlowAttribute.description = "Your hobby";
identityUserFlowAttribute.dataType = IdentityUserFlowAttributeDataType.STRING;

graphClient.identity().userFlowAttributes()
    .buildRequest()
    .post(identityUserFlowAttribute);

```