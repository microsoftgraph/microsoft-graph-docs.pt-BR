---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1ee66f332f26703bd7ea5ec0f1876c266d40842299fc277fe31ae6b2b6421700
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272408"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OrganizationalBrandingLocalizationCollectionPage localizations = graphClient.organization("d69179bf-f4a4-41a9-a9de-249c0f2efb1d").branding().localizations()
    .buildRequest()
    .get();

```