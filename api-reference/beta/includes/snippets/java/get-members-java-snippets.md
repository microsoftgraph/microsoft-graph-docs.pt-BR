---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9339680389d962e0edd9f10a3a2df6b675d7a13e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860603"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEducationUserCollectionPage members = graphClient.education().classes("11016").members()
    .buildRequest()
    .get();

```