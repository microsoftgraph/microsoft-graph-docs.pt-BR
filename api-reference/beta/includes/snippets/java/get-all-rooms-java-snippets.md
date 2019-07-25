---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 939d03cd65fc04d196f5c166d42d2a18d1a7bc1d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876739"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IRoomCollectionPage microsoft.graph.room = graphClient.places().microsoft.graph.room()
    .buildRequest()
    .get();

```