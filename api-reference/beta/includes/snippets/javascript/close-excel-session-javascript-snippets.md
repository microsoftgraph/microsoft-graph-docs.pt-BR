---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fb414e5470fe01b193c297d9b0f677e6e2288ff77403ac14c3f89e365936a0da
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899989"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const closeSession = {

};

await client.api('/me/drive/items/{id}/workbook/closeSession')
    .version('beta')
    .post(closeSession);

```