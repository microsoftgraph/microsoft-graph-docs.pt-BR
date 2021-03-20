---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b8fde85371750d11819fc47a016b0be05e3c6aa2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972684"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationRubricCollectionPage rubrics = graphClient.education().me().rubrics()
    .buildRequest()
    .get();

```