---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b21db62aa5b6483d1618617d5403f860d277d967b63c46063bb6ade94442c76e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214994"
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