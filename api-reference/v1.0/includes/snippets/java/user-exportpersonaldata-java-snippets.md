---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 13b99ca5906deb3b21f83dd9f0c127a599dfe228
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35885729"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String storageLocation = "storageLocation-value";

graphClient.users("{id}")
    .exportPersonalData(storageLocation)
    .buildRequest()
    .post();

```