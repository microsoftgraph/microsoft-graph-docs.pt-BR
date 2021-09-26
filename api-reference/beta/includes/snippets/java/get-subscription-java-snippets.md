---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e44e078f53efb54293426dd0173c3e97e14514188146b63199069d55a4e25ec3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156418"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Subscription subscription = graphClient.subscriptions("{id}")
    .buildRequest()
    .get();

```