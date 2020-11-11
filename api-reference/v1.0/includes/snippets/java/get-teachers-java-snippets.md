---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d3a39778313961e5885e3ae4b68e23ca01c21102
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48983027"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IEducationUserCollectionWithReferencesPage teachers = graphClient.education().classes("{class-id}").teachers()
    .buildRequest()
    .get();

```