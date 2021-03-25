---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a50aad25d66ca488128bb37b991f1efe4816fe3e
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210581"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserFlowLanguagePageCollectionPage overridesPages = graphClient.identity().b2cUserFlows("B2C_1_Customer").languages("en").overridesPages()
    .buildRequest()
    .get();

```