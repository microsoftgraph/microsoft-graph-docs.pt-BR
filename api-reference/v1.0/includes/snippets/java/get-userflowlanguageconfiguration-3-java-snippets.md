---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 808d80ee254773c5ff4c8171ed7100a0601bee966a685fb1dd2a4bff396abca7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275275"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserFlowLanguageConfiguration userFlowLanguageConfiguration = graphClient.identity().b2xUserFlows("B2X_1_Partner").languages("en")
    .buildRequest()
    .get();

```