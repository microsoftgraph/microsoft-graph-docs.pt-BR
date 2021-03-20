---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7079eca13dec9d20132d35634644f18a55dd67dc
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978125"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSubmissionCollectionPage submissions = graphClient.education().classes("11021").assignments("19002").submissions()
    .buildRequest()
    .get();

```