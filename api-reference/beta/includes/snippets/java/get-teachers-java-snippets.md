---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 65509381d74650add28d13ff63f7dfce9a1bcaf56b447462b0d977811893e206
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102136"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationUserCollectionWithReferencesPage teachers = graphClient.education().classes("11023").teachers()
    .buildRequest()
    .get();

```