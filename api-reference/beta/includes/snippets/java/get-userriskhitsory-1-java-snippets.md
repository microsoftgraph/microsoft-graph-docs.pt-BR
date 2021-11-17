---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 61d2fbd66420ec5d66c5cebcad96393352dff50720e2a3904c51793e7f3fb512
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157069"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RiskyUserHistoryItemCollectionPage history = graphClient.riskyUsers("41a31b00-3b3b-42d9-8f1c-6d4f14e74c69").history()
    .buildRequest()
    .get();

```