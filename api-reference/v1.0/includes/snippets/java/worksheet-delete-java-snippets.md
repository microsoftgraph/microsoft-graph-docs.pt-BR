---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b415a0fd37069a21125bf272bacbf0736b1140c88bb9d8c867fe73147b8cd7e9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329829"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().drive().items("{id}").workbook().worksheets("{id|name}")
    .buildRequest()
    .delete();

```