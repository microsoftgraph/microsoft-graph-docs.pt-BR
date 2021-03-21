---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 55144ab6ff9bb352e58fa2ea24c22f989311540b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982748"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ProgramControlCollectionPage programControls = graphClient.programControls()
    .buildRequest()
    .get();

```