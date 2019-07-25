---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 57b633f469f4abe9edba550f151b13a8c71023f3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881718"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDriveItemVersionCollectionPage versions = graphClient.me().drive().items("{item-id}").versions()
    .buildRequest()
    .get();

```