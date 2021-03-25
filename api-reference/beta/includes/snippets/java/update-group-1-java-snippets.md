---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c22e0a700fc826123b21e8b60501f57268e72a31
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210242"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Group group = new Group();
group.description = "description-value";
group.displayName = "displayName-value";

graphClient.groups("{id}")
    .buildRequest()
    .patch(group);

```