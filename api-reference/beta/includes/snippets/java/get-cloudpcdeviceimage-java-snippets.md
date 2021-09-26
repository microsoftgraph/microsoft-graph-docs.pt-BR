---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e2f7a18f12fdc441876a2c80fdb7f09d6ad1f54d034925ff1db435c8dba454df
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102539"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcDeviceImage cloudPcDeviceImage = graphClient.deviceManagement().virtualEndpoint().deviceImages("{id}")
    .buildRequest()
    .get();

```