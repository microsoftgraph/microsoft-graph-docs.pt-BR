---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cc73bfa7fedc9f3c275f3907c9ee652da73dd760
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015852"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IConnectorCollectionPage connectors = graphClient.onPremisesPublishingProfiles("applicationProxy").connectors()
    .buildRequest()
    .get();

```