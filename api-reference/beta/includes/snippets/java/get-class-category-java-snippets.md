---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ffca0545ca2991e1601579bf060bc70a842358ab
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52991672"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationCategory educationCategory = graphClient.education().classes("dacbf757-888d-42ae-b701-5e57cec300ae").assignmentCategories("7f64924d-4cdb-4e54-8c37-c0f3d46f0747")
    .buildRequest()
    .get();

```