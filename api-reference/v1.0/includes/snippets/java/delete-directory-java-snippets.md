---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 002b55b093161fae2ede68fc5c9663e331176f77
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35883307"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.directory().deletedItems("{object-id}")
    .buildRequest()
    .delete();

```