---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 85f7576a2a26bfeb5100f4240256c1eb15eaf6b7
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210749"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationClassCollectionWithReferencesPage classes = graphClient.education().schools("{school-id}").classes()
    .buildRequest()
    .get();

```