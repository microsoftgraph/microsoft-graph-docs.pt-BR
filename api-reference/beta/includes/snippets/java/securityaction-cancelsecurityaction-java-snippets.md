---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 855785be5e7440d64a0559d3cfafb9a7ac004d454cad496176487bc1dc4268c5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216153"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.security().securityActions("{id}")
    .cancelSecurityAction()
    .buildRequest()
    .post();

```