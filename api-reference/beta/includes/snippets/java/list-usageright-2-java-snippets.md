---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8b5f2376c5654f0b733b68781275e49a3362e7ac
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209244"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UsageRightCollectionPage usageRights = graphClient.devices("{objectId}").usageRights()
    .buildRequest()
    .filter("state in ('active', 'suspended') and serviceIdentifier in ('ABCD')")
    .get();

```