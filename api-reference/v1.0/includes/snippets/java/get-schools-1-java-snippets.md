---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 122a7dc34fdd9992521f223d139e707e759a1b01fb6444a1722a12c3f4868f57
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56897823"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSchoolCollectionWithReferencesPage schools = graphClient.education().classes("{class-id}").schools()
    .buildRequest()
    .get();

```