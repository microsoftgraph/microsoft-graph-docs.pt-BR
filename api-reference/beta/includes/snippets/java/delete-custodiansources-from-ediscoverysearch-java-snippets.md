---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9892bd1befb8820dcea7218b0d753d9b78407f89
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092065"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.security().cases().ediscoveryCases("{ediscoveryCaseId}").searches("{ediscoverySearchId}").custodianSources("{id}").reference()
    .buildRequest()
    .delete();

```