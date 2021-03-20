---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 874e85507a6c3f79a95f9f1e4a445433d2a19c3c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944624"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserFlowLanguageConfiguration userFlowLanguageConfiguration = new UserFlowLanguageConfiguration();
userFlowLanguageConfiguration.id = "es-ES";
userFlowLanguageConfiguration.isEnabled = true;

graphClient.identity().b2cUserFlows("B2C_1_CustomerSignUp").languages("es-ES")
    .buildRequest()
    .put(userFlowLanguageConfiguration);

```