---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 92fbbc674533dff6835e90fe05706ed37ba20a2055dcc56b8c903dc20d85ab15
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57271869"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AudioRoutingGroupCollectionPage audioRoutingGroups = graphClient.communications().calls("{id}").audioRoutingGroups()
    .buildRequest()
    .get();

```