---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: af195a7d64e798758770867d3e1449f157957bddcd3522db705075e7c217cbb5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56900241"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConnectorGroupCollectionPage connectorGroups = graphClient.onPremisesPublishingProfiles("applicationProxy").connectorGroups()
    .buildRequest()
    .get();

```