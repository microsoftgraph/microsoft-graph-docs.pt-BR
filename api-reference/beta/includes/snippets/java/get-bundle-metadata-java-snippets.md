---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 44047980d86eb66e5b7e75e6b517fcd1c9061543a0be7b8e80cf7acb71c17f03
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102170"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

DriveItem driveItem = graphClient.drive().bundles("{bundle-id}")
    .buildRequest()
    .get();

```