---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c2beee86bd5df95c2cb261a651483888e1fc4ad5
ms.sourcegitcommit: c75356177c73ec480cec868a4404a63dca5b078d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/15/2020
ms.locfileid: "43512291"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{site-id}/lists/{list-title}')
    .get();

```