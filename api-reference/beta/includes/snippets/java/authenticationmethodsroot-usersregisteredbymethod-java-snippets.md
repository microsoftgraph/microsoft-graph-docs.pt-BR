---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 14249137635c25a29e416b87cec9bdcaa02ea103
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2021
ms.locfileid: "50092366"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UserRegistrationMethodSummary userRegistrationMethodSummary = graphClient.reports().authenticationMethods()
    .usersRegisteredByMethod('all','all')
    .buildRequest()
    .get();

```