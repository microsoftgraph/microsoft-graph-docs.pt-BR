---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 186747c39d5215164783549f81869ddcc2b1ea5e5399c20d3adf06f72edc88ae
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899788"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSchoolDeltaCollectionPage delta = graphClient.education().schools()
    .delta()
    .buildRequest()
    .get();

```