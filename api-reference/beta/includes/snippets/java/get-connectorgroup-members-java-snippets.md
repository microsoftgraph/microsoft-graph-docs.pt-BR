---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d5c908ace11407eb5cfc28171c63f5174709485b
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2022
ms.locfileid: "65719089"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConnectorCollectionWithReferencesPage members = graphClient.onPremisesPublishingProfiles("applicationProxy").connectorGroups("{id}").members()
    .buildRequest()
    .get();

```