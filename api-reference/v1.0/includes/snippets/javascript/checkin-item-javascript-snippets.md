---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6cb64fef5bfab6a57c9ed1b821de29fa987bfbab3d704b0c868ab94c0bf4ac4f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57407699"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const checkin = {
  comment: 'Updating the latest guidelines'
};

await client.api('/drives/{drive-id}/items/{item-id}/checkin')
    .post(checkin);

```