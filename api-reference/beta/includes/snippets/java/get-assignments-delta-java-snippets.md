---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8556d1a9e2a25fd50b2bd84f056acc8c89b7ec39
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137556"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentDeltaCollectionPage delta = graphClient.education().classes("72a7baec-c3e9-4213-a850-f62de0adad5f").assignments()
    .delta()
    .buildRequest()
    .get();

```