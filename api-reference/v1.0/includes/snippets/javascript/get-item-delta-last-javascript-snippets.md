---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1187fa62a43c7ad285a869b3591773ae7f4c6b0ac8e5647e7ab9ac976a366524
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100275"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/me/drive/root/delta(token='1230919asd190410jlka')')
    .get();

```