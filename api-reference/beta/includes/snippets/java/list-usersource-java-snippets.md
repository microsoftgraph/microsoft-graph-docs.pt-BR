---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: df112a18d6f8f89b0bf8c5f451684f9be615c459
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773036"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IUserSourceCollectionPage userSources = graphClient.compliance().ediscovery().cases("c816dd6f-5af8-40c5-a760-331361e05c60").legalHolds("277107ff-fee3-41a0-a665-a9d7f6c4824f").userSources()
    .buildRequest()
    .get();

```