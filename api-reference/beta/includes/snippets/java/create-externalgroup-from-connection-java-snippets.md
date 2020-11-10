---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 353ef2ca7a5429a8b92a454bba0ab60cfddc261a
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965612"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ExternalGroup externalGroup = new ExternalGroup();
externalGroup.id = "31bea3d537902000";
externalGroup.displayName = "Contoso Marketing";
externalGroup.description = "The product marketing team";

graphClient.external().connections("contosohr").groups()
    .buildRequest()
    .post(externalGroup);

```