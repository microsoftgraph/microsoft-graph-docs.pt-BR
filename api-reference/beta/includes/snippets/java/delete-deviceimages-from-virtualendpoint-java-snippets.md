---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 08129879f651c8e203502f0bf1e922c24979f816a7e0375c0c080c295198d89b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099408"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.deviceManagement().virtualEndpoint().deviceImages("{id}")
    .buildRequest()
    .delete();

```