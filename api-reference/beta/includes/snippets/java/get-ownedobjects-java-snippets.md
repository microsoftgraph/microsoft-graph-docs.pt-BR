---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 53fd2d08e445dba9b63d19b1fb03ceabd8b80aa6
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015510"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDirectoryObjectCollectionWithReferencesPage ownedObjects = graphClient.servicePrincipals("{id}").ownedObjects()
    .buildRequest()
    .get();

```