---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cee953866b593dcd90024bdaf206fd851a90792b
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/29/2019
ms.locfileid: "34535984"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drive/items/{item-id}/content?format=%7Bformat%7D')
    .version('beta')
    .get();

```