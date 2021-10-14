---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 47dd6ca195cd796af1875ef213a0fe58f0d13a429bccb91a843cb94cf1e80fa9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57376580"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.servicePrincipals("{id}")
    .buildRequest()
    .delete();

```