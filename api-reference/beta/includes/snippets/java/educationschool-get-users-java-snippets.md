---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2164309ac423b11fc59ca02348c847f2301432e7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48955525"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEducationUserCollectionWithReferencesPage users = graphClient.education().schools("10002").users()
    .buildRequest()
    .get();

```