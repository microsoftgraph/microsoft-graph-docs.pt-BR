---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d12bfc76f8739e11f377bae89733341c59349c52
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441466"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcDeviceCollectionPage cloudPcDevices = graphClient.tenantRelationships().managedTenants().cloudPcDevices()
    .buildRequest()
    .get();

```