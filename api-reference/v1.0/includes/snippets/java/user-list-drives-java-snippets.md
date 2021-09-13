---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 588e45ab41ea7c6072e79683c4f929e5f0c8509f2ad5d546581a3416ffe5dec8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158984"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveCollectionPage drives = graphClient.users("{userId}").drives()
    .buildRequest()
    .get();

```