---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ff52e1da245308d3b064671c4bbb2a5c795abe1a
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333640"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.teams("{id}")
    .unarchive()
    .buildRequest()
    .post();

```