---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3843244067846da555809c7034b138df479e00bb
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240984"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewPolicy accessReviewPolicy = graphClient.policies().accessReviewPolicy()
    .buildRequest()
    .get();

```