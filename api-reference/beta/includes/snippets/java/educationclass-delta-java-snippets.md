---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 42bc323e9d49c86fea7ef16c7dbdf856c8f44d8e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50984288"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationClassDeltaCollectionPage delta = graphClient.education().classes()
    .delta()
    .buildRequest()
    .get();

```