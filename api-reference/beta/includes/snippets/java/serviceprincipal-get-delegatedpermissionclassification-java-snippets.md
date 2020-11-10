---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 942a3945cd053e00c710cc777dd9dc21be97cee6
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980567"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IDelegatedPermissionClassificationCollectionPage delegatedPermissionClassifications = graphClient.servicePrincipals("{id}").delegatedPermissionClassifications()
    .buildRequest()
    .get();

```