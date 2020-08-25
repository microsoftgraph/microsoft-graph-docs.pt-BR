---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 59a2fa7828f393c6583e5ba4b5d3ab9713835377
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873935"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root/search(q='Contoso Projec}')')
    .version('beta')
    .get();

```