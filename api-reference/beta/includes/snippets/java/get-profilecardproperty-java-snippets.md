---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 06f176ed59a814b9dd5a0b625cc20e0ccff3eacc
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48980842"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ProfileCardProperty profileCardProperty = graphClient.organization("{organizationId}").settings().profileCardProperties("{id}")
    .buildRequest()
    .get();

```