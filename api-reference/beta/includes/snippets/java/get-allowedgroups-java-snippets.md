---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8887c38742adc4bc45b99b89433dc2a021fa68ba
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976989"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GroupCollectionWithReferencesPage allowedGroups = graphClient.print().shares("{id}").allowedGroups()
    .buildRequest()
    .get();

```