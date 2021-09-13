---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 05e8758d09470661370747c82cb19e3df497ec08
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59147558"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.sites("{site-id}").contentTypes("{contentType-id}")
    .buildRequest()
    .delete();

```