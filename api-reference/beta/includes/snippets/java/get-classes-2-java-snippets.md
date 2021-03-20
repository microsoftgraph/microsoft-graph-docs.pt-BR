---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 72cd72ca93c34a13683fdc74e7609f6e10dab66c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951322"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEducationClassCollectionWithReferencesPage classes = graphClient.education().schools("10002").classes()
    .buildRequest()
    .get();

```