---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6526037c221ae232fb54dae01d065d9d5507ae1d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881521"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEducationUserCollectionPage teachers = graphClient.education().classes("{class-id}").teachers()
    .buildRequest()
    .get();

```