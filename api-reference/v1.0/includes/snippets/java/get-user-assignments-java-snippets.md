---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d60f79968d0a5f39ade15f1a1e3618414ae2afee
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62111054"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentCollectionPage assignments = graphClient.education().users("f3a5344e-dbde-48b0-be24-b5b62a243836").assignments()
    .buildRequest()
    .get();

```