---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b050fbca2d927801246228ff2ab6286c9c64d32aee3d3be4843b63d0b55b1b4a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102658"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendar = {
  name: 'Social events'
};

await client.api('/me/calendar')
    .version('beta')
    .update(calendar);

```