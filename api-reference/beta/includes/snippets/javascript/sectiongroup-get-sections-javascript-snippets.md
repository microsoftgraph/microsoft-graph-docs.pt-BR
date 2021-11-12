---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c22d7c8a952a990c423d6459094aae1dc917d0b404da05216c9a9f7f6944626e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216306"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sections = await client.api('/me/onenote/sectionGroups/{id}/sections')
    .version('beta')
    .get();

```