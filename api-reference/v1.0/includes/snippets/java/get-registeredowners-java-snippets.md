---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6eacd581addc3419c72b83a7af7326ea70e2f93a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977541"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage registeredOwners = graphClient.devices("{id}").registeredOwners()
    .buildRequest()
    .get();

```