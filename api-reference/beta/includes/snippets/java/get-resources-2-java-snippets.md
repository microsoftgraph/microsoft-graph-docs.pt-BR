---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 27b83d8034adca6476805863d16d8e922024b02e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50951255"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEducationSubmissionResourceCollectionPage resources = graphClient.education().classes("{id}").assignments("{id}").submissions("{id}").resources()
    .buildRequest()
    .get();

```