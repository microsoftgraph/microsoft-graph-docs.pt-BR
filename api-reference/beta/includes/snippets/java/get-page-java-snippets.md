---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5216a2169c30750330a186a825237b1fc889f23c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869565"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SitePage sitePage = graphClient.sites("{site-id}").pages("{page-id}")
    .buildRequest()
    .get();

```