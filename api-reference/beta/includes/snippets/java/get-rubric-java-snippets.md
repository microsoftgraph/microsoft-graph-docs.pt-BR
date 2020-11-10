---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e98d4ee4e25308c7eeaf52a42d983fe4b094f70e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48966583"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationRubric educationRubric = graphClient.education().me().assignments("{id}").rubric()
    .buildRequest()
    .get();

```