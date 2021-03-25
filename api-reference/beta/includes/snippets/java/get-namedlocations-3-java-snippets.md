---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5a127e61b15d7788f329508f5d6f4a48ada1673f
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210719"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

NamedLocationCollectionPage namedLocations = graphClient.identity().conditionalAccess().namedLocations()
    .buildRequest()
    .filter("createdDateTime ge 2019-09-01T00:00:00Z")
    .get();

```