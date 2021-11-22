---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9517f3fd0cd6e6dad168ffe4129d0b23f1e509cdbe404bbe964a3e9442510f39
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273183"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TokenLifetimePolicyCollectionPage tokenLifetimePolicies = graphClient.policies().tokenLifetimePolicies()
    .buildRequest()
    .get();

```