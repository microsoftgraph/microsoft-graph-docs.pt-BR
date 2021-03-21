---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0af553420c62eb8b4d8815d49fa26116879e8b39
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50984374"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage memberOf = graphClient.users("{id}").memberOf()
    .buildRequest()
    .get();

```