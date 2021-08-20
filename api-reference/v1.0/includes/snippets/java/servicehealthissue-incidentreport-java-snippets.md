---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: da1146fe51387095ea1a1cceacbec54477d5c83e
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58266134"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

InputStream stream = graphClient.admin().serviceAnnouncement().issues("MO248163")
    .incidentReport()
    .buildRequest()
    .get();

```