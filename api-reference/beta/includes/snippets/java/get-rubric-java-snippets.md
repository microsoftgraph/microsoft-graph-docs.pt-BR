---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 470faeb478736e9be6a03e5fd97d3f06fb18faa3
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52254225"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationRubric educationRubric = graphClient.education().classes("{id}").assignments("{id}").rubric()
    .buildRequest()
    .get();

```