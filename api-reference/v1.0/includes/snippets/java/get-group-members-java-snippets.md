---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c3f43e44fad733d1e8d164eeb6fd24e1fa12f110
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967973"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage members = graphClient.groups("{id}").members()
    .buildRequest()
    .get();

```