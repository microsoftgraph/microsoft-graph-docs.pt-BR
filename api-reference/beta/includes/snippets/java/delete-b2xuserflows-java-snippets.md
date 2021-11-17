---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 757e0b0a32a16dcb4a890322a921376e39efc4558c13de4468c64d7b1e40f04a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899448"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identity().b2xUserFlows("{id}")
    .buildRequest()
    .delete();

```