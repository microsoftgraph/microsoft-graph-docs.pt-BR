---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 259895ebe009d0a0b9a5a7421a0699a0b83377b7
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52254244"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationOutcomeCollectionPage outcomes = graphClient.education().classes("{id}").assignments("{id}").submissions("{id}").outcomes()
    .buildRequest()
    .get();

```