---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d10f78287d70d790c8541156760c04625790a124
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884133"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IGroupSettingCollectionPage groupSettings = graphClient.groupSettings()
    .buildRequest()
    .get();

```