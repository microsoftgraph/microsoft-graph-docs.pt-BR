---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7f91a38af000ef995a59b2cb2bca65b1788ef401
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35894010"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().activities("{activity-id}")
    .buildRequest()
    .delete();

```