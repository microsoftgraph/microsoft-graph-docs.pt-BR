---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fee379e9468d5ae249bcf01dcc587bed63981a5e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955243"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserFlowLanguageConfiguration userFlowLanguageConfiguration = graphClient.identity().b2cUserFlows("B2C_1_Customer").languages("en")
    .buildRequest()
    .get();

```