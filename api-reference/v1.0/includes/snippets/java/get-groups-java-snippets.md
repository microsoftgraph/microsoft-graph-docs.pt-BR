---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7952b4528c31aef6dfd78f5b548642a22b81bcaa
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888990"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IGroupCollectionPage groups = graphClient.groups()
    .buildRequest()
    .get();

```