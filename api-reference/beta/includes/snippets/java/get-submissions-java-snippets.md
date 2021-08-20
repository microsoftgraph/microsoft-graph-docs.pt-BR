---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 38ab886d4c9335c62088b2ab5277b738b02ef57e5183c2237fc48b3a96f61489
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157011"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSubmissionCollectionPage submissions = graphClient.education().classes("11021").assignments("19002").submissions()
    .buildRequest()
    .get();

```