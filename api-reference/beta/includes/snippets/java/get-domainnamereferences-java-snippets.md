---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e76553bf5b58b6f63e7997d00b6f9c4f32a4a63f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973276"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage domainNameReferences = graphClient.domains("contoso.com").domainNameReferences()
    .buildRequest()
    .get();

```