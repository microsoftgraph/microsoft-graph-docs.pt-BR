---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b49b509774ccfaf067a799512ad9e8b510dc9348
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967917"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConnectorGroupCollectionPage memberOf = graphClient.onPremisesPublishingProfiles("applicationProxy").connectors("{id}").memberOf()
    .buildRequest()
    .get();

```