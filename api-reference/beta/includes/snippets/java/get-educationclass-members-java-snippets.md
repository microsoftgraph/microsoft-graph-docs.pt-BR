---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 04fdea0ba91257221c22ef0fb88c2765b5e60754
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980994"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUserCollectionWithReferencesPage members = graphClient.education().classes("11016").members()
    .buildRequest()
    .get();

```