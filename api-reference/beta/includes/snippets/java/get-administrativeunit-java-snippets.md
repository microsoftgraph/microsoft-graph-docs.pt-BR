---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ce72c5413d97e96580df35cf289c71567f4abd8b
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63351060"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AdministrativeUnit administrativeUnit = graphClient.administrativeUnits("4d7ea995-bc0f-45c0-8c3e-132e93bf95f8")
    .buildRequest()
    .get();

```