---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ddd00acb36bcb5691969e3ebca5f5b7eeef8ffe4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970963"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUserDeltaCollectionPage delta = graphClient.education().users()
    .delta()
    .buildRequest()
    .get();

```