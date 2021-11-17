---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e19a87ace292210b6107832bed344d6e1238b95fff0136e68e6a4b47f61ecb95
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898066"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().termsOfUse().agreements("{id}")
    .buildRequest()
    .delete();

```