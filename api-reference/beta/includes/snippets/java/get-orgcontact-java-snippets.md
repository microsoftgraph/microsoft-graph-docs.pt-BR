---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 95c020a32b102856f43c67228d44ba98c90acd1b
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877915"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OrgContact orgContact = graphClient.contacts("{id}")
    .buildRequest()
    .get();

```