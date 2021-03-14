---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b1beafbb3d5f55d16a48ee55db0be3fd4a4ceb4b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803093"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().schools("{school-id}").classes("{class-id}")
    .buildRequest()
    .delete();

```