---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7146b587645ec32ce2f076e638d775f34a3672e2823bb010ed4a466f5ff88f69
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157447"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserFlowLanguageConfiguration userFlowLanguageConfiguration = new UserFlowLanguageConfiguration();
userFlowLanguageConfiguration.isEnabled = false;

graphClient.identity().b2cUserFlows("B2C_1_CustomerSignUp").languages("es-ES")
    .buildRequest()
    .put(userFlowLanguageConfiguration);

```