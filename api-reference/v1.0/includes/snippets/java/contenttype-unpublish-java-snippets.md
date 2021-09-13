---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3073e2a505f2875d473f8b4e33ab032e02e49937
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59038103"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.sites("{siteId}").contentTypes("{contentTypeId}")
    .unpublish()
    .buildRequest()
    .post();

```