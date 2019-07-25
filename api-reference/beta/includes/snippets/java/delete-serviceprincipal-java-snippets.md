---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 84c5cbceae977e826c4faa3140a1db142fadf061
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35870209"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.servicePrincipals("{id}")
    .buildRequest()
    .delete();

```