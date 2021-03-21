---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b1beafbb3d5f55d16a48ee55db0be3fd4a4ceb4b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956594"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.education().schools("{school-id}").classes("{class-id}")
    .buildRequest()
    .delete();

```