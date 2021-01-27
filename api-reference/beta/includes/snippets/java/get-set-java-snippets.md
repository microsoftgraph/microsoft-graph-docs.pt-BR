---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5053606b9e1604404ad31c98cd6c705f21c429f9
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015643"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISetCollectionPage sets = graphClient.termStore().groups("{groupId}").sets()
    .buildRequest()
    .get();

```