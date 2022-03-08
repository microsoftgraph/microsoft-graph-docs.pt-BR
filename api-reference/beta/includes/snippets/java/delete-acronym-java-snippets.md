---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c3737090c178fca2881b5a87604518970de80e75
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338434"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.search().acronyms("{acronymsId}")
    .buildRequest()
    .delete();

```