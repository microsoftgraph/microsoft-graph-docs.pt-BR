---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0943075bd69b8f397b91c87964281fe8ee35a283
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50981726"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DirectoryObjectCollectionWithReferencesPage directReports = graphClient.me().directReports()
    .buildRequest()
    .get();

```