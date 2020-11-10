---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f3d75e1c8ca7264be46422af6f7476b938947c3a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48951486"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IContactCollectionPage contacts = graphClient.me().contacts()
    .buildRequest()
    .select("displayName,emailAddresses")
    .get();

```