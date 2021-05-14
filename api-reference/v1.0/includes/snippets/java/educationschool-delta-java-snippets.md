---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 303f07487e744ed067883482d19dfbf430158246
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474917"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSchoolDeltaCollectionPage delta = graphClient.education().schools()
    .delta()
    .buildRequest()
    .get();

```