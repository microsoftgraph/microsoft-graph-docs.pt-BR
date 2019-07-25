---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d0473a1299f3843753e045285f5a654f354f0a4c
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35870272"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ISecurityActionCollectionPage securityActions = graphClient.security().securityActions()
    .buildRequest()
    .get();

```