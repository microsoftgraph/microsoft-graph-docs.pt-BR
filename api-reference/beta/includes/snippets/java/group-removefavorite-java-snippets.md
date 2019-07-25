---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 84f40b63c3f48ecbba0a5134f0cef3d5b431b84a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857924"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.groups("{id}")
    .removeFavorite()
    .buildRequest()
    .post();

```