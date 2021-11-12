---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7bbb31d1009fbab7e7654b3ea3310e0ad9270aad68256d62a0ea95eccfa31d61
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101945"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/Range')
    .version('beta')
    .get();

```