---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bf363bf3ae61b5eb51e1e703d6ee2a705da8198a
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2020
ms.locfileid: "43184234"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/applications/{id}/owners/{id}/$ref')
    .version('beta')
    .delete();

```