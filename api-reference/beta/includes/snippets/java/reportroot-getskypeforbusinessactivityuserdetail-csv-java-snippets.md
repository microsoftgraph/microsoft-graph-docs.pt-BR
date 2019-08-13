---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 05537593a32aba71ec33fb06866ab678cbd72d50
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36359431"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISkypeForBusinessActivityUserDetailCollectionPage getSkypeForBusinessActivityUserDetail = graphClient.reports()
    .getSkypeForBusinessActivityUserDetail("D7")
    .buildRequest()
    .get();

```