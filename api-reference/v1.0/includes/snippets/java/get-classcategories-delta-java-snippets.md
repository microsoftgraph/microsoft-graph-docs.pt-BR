---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f4e14384fd11885080edca25c9d707199ee85725
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629392"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationCategoryDeltaCollectionPage delta = graphClient.education().classes("72a7baec-c3e9-4213-a850-f62de0adad5f").assignmentCategories()
    .delta()
    .buildRequest()
    .get();

```