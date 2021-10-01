---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 21b52bd3ccbb257b9159d5bc1e0dee082a6e7f9f0fa45b70713ef550f8480b55
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327841"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationSynchronizationProfile educationSynchronizationProfile = graphClient.education().synchronizationProfiles("{id}")
    .buildRequest()
    .get();

```