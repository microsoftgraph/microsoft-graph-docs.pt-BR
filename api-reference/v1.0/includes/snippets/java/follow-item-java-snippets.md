---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cb1d8e2e71a0aade9a7e2595ac333ffabaed028f
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2020
ms.locfileid: "43124382"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{item-id}")
    .follow()
    .buildRequest()
    .post();

```