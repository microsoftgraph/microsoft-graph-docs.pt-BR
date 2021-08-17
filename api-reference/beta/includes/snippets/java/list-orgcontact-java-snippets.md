---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b490464b711176bdcb668bf3ffd22324e46afebfdccf4805dc75364b26cbd89f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214102"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OrgContactCollectionPage contacts = graphClient.contacts()
    .buildRequest()
    .get();

```