---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5215f60d46629ce52ad9a7ace2a4ee13a25a6fb27bedcb715b523dcc3bcc2f64
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102389"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let subscription = await client.api('/subscriptions/{id}')
    .get();

```