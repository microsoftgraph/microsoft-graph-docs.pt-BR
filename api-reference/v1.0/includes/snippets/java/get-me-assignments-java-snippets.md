---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e146ffe9b57617a960ba504d1fa80ca0e7bea20b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62111052"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentCollectionPage assignments = graphClient.education().me().assignments()
    .buildRequest()
    .get();

```