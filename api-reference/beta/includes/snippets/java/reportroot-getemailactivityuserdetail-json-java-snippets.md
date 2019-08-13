---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d6d8d9018ca743975b5d4cf6f80c9e974a0227d4
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36308456"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEmailActivityUserDetailCollectionPage getEmailActivityUserDetail = graphClient.reports()
    .getEmailActivityUserDetail("D7")
    .buildRequest()
    .get();

```