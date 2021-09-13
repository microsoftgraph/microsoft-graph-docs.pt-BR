---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a4aaac7fb2099a1014ba9ea03b26a8f1282a7d43d728588b18a15b476a86e09a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214248"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let names = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/names')
    .get();

```