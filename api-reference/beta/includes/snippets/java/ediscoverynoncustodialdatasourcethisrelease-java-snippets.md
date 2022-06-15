---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 62ab985cec257dd1e1621986c3af8e2b6ff1020f
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092199"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.security().cases().ediscoveryCases("{ediscoveryCaseId}").noncustodialDataSources("{ediscoveryNoncustodialDataSourceId}")
    .release()
    .buildRequest()
    .post();

```