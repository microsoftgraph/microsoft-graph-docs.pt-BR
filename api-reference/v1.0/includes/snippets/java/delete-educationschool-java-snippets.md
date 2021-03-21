---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ede143e1d9f7fdcdcb7a08b95a4fd4ec8c23e6b2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980527"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().schools("{school-id}")
    .buildRequest()
    .delete();

```