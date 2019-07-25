---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b71bcff71239057481174b294482ef8babf5a61d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884846"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationRoot educationRoot = graphClient.education()
    .buildRequest()
    .get();

```