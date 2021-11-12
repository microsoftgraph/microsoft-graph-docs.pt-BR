---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eb08edd4b69024b661285c3932c0bcc4a3f325908643c7199f428c8bd5dddeac
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217356"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tables = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/tables')
    .version('beta')
    .get();

```