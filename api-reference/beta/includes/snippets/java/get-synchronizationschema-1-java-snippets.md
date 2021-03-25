---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3876063b18a122410f751b3ae000645e38e1c7ce
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210027"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SynchronizationSchema synchronizationSchema = graphClient.servicePrincipals("{id}").synchronization().jobs("{jobId}").schema()
    .buildRequest()
    .get();

```