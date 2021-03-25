---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d9e05883012f08cf315f72c4eec5b44677d7fa3b
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210852"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage ownedObjects = graphClient.servicePrincipals("{id}").ownedObjects()
    .buildRequest()
    .get();

```