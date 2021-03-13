---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 684abe2ca0b5bfbc2c0c827918d8a327474e4d0e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776673"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ICaseOperationCollectionPage operations = graphClient.compliance().ediscovery().cases("061b9a92-8926-4bd9-b41d-abf35edc7583").operations()
    .buildRequest()
    .get();

```