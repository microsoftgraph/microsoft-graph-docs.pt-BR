---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2594fed89a9120b3e26b61d023eb0c79defe2955
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50971210"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage memberOf = graphClient.devices("{id}").memberOf()
    .buildRequest()
    .get();

```