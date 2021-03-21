---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bada49b9ac872f095a0b945837ae7cd7d1adf876
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968133"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

User user = graphClient.users("{id}")
    .buildRequest()
    .get();

```