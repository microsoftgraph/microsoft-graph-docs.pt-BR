---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9b39d331b4c874812628b23e3e0f41ee914ed33d
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015796"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEducationSchoolCollectionWithReferencesPage schools = graphClient.education().classes("11014").schools()
    .buildRequest()
    .get();

```