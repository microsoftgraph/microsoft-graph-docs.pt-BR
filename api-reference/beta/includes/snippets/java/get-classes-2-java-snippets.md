---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6ac05bae08eaf6110f21d70c5a409696f225b971
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51211013"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationClassCollectionWithReferencesPage classes = graphClient.education().schools("10002").classes()
    .buildRequest()
    .get();

```