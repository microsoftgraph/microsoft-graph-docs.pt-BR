---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 85deb44f1a07afcb3857b70385c1e39ce1ba8b123feefda81a9027fbeda48ad0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216992"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ContentType contentType = graphClient.sites("{site-id}").contentTypes("{contentType-id}")
    .buildRequest()
    .get();

```