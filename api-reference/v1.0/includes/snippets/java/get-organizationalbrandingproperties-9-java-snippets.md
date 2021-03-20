---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bb973e4c8695b42eb1c4724d23da146d0e1d0f0c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50949195"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOrganizationalBrandingLocalizationCollectionPage localizations = graphClient.organization("d69179bf-f4a4-41a9-a9de-249c0f2efb1d").branding().localizations()
    .buildRequest()
    .get();

```