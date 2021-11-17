---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4a9e3ccfb4d3cac439e97772e9064ac1d3a493c34cc4bb199de8f7aece368bf7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327284"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TokenLifetimePolicy tokenLifetimePolicy = graphClient.policies().tokenLifetimePolicies("{id}")
    .buildRequest()
    .get();

```