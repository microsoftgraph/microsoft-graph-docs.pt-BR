---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 31cc8cbed45f62b0d3a8d2fb4d0a2e55471ea9ee126f7d0819eec14d8f8fc08d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898921"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let applicationTemplate = await client.api('/applicationTemplates/{id}')
    .version('beta')
    .get();

```