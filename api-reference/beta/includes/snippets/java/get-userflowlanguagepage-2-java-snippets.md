---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 44d977de91244e34f79a9c80bb4418801f8ed15e8507f639119e380373b7d815
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100325"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserFlowLanguagePageCollectionPage overridesPages = graphClient.identity().b2cUserFlows("B2C_1_Customer").languages("en").overridesPages()
    .buildRequest()
    .get();

```