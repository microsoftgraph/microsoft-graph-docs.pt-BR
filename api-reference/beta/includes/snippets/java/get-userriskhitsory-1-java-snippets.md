---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 102878365fab0e079f5055f1be2b69dc1e7272f8
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208344"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RiskyUserHistoryItemCollectionPage history = graphClient.riskyUsers("41a31b00-3b3b-42d9-8f1c-6d4f14e74c69").history()
    .buildRequest()
    .get();

```