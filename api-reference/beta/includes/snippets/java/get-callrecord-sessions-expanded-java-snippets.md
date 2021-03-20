---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 84b5c3c623f8d194e0a4df97b07b56fdfbf1dedb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973942"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SessionCollectionPage sessions = graphClient.communications().callRecords("{id}").sessions()
    .buildRequest()
    .expand("segments")
    .get();

```