---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 37524563a32bc202166231fa1f973a9c193e11e330d83b1a395bb05977735cf5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100197"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/communications/calls/{id}/audioRoutingGroups/{id}')
    .version('beta')
    .delete();

```