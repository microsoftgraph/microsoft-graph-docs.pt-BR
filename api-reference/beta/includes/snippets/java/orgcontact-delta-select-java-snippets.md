---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b3e6223803d987bc1a2305f18e67836ffd468674
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48974293"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOrgContactDeltaCollectionPage delta = graphClient.contacts()
    .delta()
    .buildRequest()
    .select("displayName,jobTitle,mail")
    .get();

```