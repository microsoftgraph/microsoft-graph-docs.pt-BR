---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 548c6134ded795ef41a0712fcc5eb82579125805
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861436"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String comment = "Updating the latest guidelines";

graphClient.drives("{drive-id}").items("{item-id}")
    .checkin(checkInAs,comment)
    .buildRequest()
    .post();

```