---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 35d129d2d7f647f32e740e0b2f6847867e6fffa0
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891195"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDriveItemCollectionPage children = graphClient.drives("{drive-id}").items("{item-id}").children()
    .buildRequest()
    .get();

```