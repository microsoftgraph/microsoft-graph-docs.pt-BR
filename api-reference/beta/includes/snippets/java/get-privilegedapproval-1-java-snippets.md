---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: afa1284bc87ea1d580084d18dd8e6cc54ba2ddef
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957248"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedApproval privilegedApproval = graphClient.privilegedApproval("{id}")
    .buildRequest()
    .get();

```