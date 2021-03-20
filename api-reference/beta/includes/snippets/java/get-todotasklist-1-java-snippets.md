---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c07e599e0314151bbe9b31c4f2d043a2edfab5e7
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953807"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ITodoTaskListCollectionPage lists = graphClient.me().todo().lists()
    .buildRequest()
    .get();

```