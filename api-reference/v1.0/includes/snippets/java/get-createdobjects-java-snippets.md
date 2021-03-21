---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eb16a53f918eb23a10713bbe153a1a012a5d0aa4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972601"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage createdObjects = graphClient.me().createdObjects()
    .buildRequest()
    .get();

```