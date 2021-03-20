---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e017211de1c214d042ded04dbabb68cb83601999
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50977769"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage members = graphClient.directoryRoles("{id}").members()
    .buildRequest()
    .get();

```