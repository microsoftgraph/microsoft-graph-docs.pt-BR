---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 41151ea77ceab2a21082258fed52d6c70c65dc89686e4f3a28c5712c68799e95
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159729"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let columns = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns')
    .get();

```