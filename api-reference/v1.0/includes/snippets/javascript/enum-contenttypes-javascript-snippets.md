---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7ac26daf40e0749dfaf8dd67ef706dbbfc6f7192
ms.sourcegitcommit: ddeee0eec277df06d9e635e5b5c257d14c856273
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2021
ms.locfileid: "60783007"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contentTypes = await client.api('/sites/{site-id}/lists/{list-id}/contentTypes')
    .get();

```