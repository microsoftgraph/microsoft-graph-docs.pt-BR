---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 606768852046a05c9c1ea6a1aa1a0b3de95a2c98
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48979435"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.servicePrincipals("{id}").delegatedPermissionClassifications("{id}")
    .buildRequest()
    .delete();

```