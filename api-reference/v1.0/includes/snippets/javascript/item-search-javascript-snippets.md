---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 76c0e8b2cf12e6af38352539c4dc69d11a385a46
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873870"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/root/search(q='Contoso Project')')
    .get();

```