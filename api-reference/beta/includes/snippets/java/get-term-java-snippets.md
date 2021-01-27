---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 63eb9f8f55b9f3889b2be559292b6716b6f01e5c
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015340"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Term term = graphClient.termStore().groups("{groupId}").sets("{setId}").terms("{termId}")
    .buildRequest()
    .get();

```