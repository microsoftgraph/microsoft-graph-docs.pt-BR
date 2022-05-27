---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 66f6d1bb5ca3b1c5bcbd13a31b5d12b98d0b7e31584cbb45757f3ac6353050ae
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216777"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationRubric educationRubric = new EducationRubric();
educationRubric.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/v1.0/education/me/rubrics/{id}"));

graphClient.education().classes("{id}").assignments("{id}").rubric().reference()
    .buildRequest()
    .put(educationRubric);

```