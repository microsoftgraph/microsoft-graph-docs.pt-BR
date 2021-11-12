---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c104d4fdf7729eb5b53bbd43ad4be931df22710edb48d2d76dd3cf89fca7700a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159982"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUser educationUser = new EducationUser();
educationUser.additionalDataManager().put("@odata.id", new JsonPrimitive("https://graph.microsoft.com/beta/education/users/14011"));

graphClient.education().classes("11017").teachers().references()
    .buildRequest()
    .post(educationUser);

```