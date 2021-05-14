---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5e8af4a9a56162487bd5ba7f144341c3b394db99
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474847"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AdministrativeUnit administrativeUnit = graphClient.education().classes("{educationClassId}").members("{educationUserId}").schools("{educationSchoolId}").administrativeUnit()
    .buildRequest()
    .get();

```