---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 961021aad0da56651c14ce5f266d12c7c7a767d2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978543"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserFlowApiConnectorConfiguration userFlowApiConnectorConfiguration = graphClient.customRequest("/identity/b2xUserFlows/B2X_1_testuserflow/apiConnectorConfiguration", UserFlowApiConnectorConfiguration.class)
    .buildRequest()
    .get();

```