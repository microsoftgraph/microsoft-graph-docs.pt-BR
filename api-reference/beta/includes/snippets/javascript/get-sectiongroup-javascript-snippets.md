---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 46d12eb144dd542943d24328769f99a888e257376be3417d0dad984735e7c94c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216682"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sectionGroup = await client.api('/me/onenote/sectionGroups/{id}')
    .version('beta')
    .get();

```