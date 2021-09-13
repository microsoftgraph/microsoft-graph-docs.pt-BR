---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 317660af16f0d51ac3f882f2b0e39e1e16f0ec894552727aeb93d0ff2956bcf1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57406755"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AdministrativeUnit administrativeUnit = graphClient.education().classes("{educationClassId}").members("{educationUserId}").schools("{educationSchoolId}").administrativeUnit()
    .buildRequest()
    .get();

```