---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 515c604fb95464190e9c46bd59f2a55dbb342d57382d79da5f1682f29e6bd08f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157928"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Endpoint endpoint = graphClient.groups("{id}").endpoints("{id}")
    .buildRequest()
    .get();

```