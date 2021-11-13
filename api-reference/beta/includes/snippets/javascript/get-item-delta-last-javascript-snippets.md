---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 49d0a4a54430414f01a54528bb64dda9240e0d74b482696d736f6001d8de25e5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102523"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/me/drive/root/delta(token='1230919asd190410jlka')')
    .version('beta')
    .get();

```