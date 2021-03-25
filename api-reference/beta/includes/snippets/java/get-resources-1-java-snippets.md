---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c4eacb65fac572054405ca68285b60410d11d050
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209120"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentResourceCollectionPage resources = graphClient.education().classes("11012").assignments("19002").resources()
    .buildRequest()
    .get();

```