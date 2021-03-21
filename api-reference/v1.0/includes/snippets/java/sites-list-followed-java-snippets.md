---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cc3ba5018689180594ee16cb5460648a989ba7cf
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976818"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SiteCollectionWithReferencesPage followedSites = graphClient.me().followedSites()
    .buildRequest()
    .get();

```