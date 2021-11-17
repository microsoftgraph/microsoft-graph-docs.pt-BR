---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a56aef0a8679365ca8b503a209d12ff16859560736eace2f186aa1c838b4c4ea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272270"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.servicePrincipals("{id}").synchronization().jobs("{jobId}")
    .buildRequest()
    .delete();

```