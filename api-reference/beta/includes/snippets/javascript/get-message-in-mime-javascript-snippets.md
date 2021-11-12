---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e367dbebe7e76b8904be710aa1601682deebff39d216d3d6e0bec5117b5630d5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275044"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/me/messages/4aade2547798441eab5188a7a2436bc1/$value')
    .version('beta')
    .get();

```