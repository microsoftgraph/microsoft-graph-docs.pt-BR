---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 453cb11860701fba2982fa74beda66db58c78e42
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48975054"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PersonInterest personInterest = new PersonInterest();
LinkedList<String> categoriesList = new LinkedList<String>();
categoriesList.add("Sports");
personInterest.categories = categoriesList;

graphClient.me().profile().interests("{id}")
    .buildRequest()
    .patch(personInterest);

```