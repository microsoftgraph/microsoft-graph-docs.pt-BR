---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 68e2594b5e92d7ea435181fa6ece9cefc8413502
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968945"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSchool educationSchool = new EducationSchool();
educationSchool.displayName = "Fabrikam Arts High School";
educationSchool.description = "Magnate school for the arts. Los Angeles School District";

graphClient.education().schools("{school-id}")
    .buildRequest()
    .patch(educationSchool);

```