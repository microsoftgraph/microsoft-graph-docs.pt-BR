---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c3c03642b66e2ce5350289ea5d799a24a5e9de3c
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210614"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSchoolCollectionWithReferencesPage schools = graphClient.education().classes("{class-id}").schools()
    .buildRequest()
    .get();

```