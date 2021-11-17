---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dae85ff77f77e1e0f3b7d1bb75dc87f850aeeccd833cf55374b5d5b3223bc4ba
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899914"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SitePage sitePage = graphClient.sites("{site-id}").pages("{page-id}")
    .buildRequest()
    .get();

```