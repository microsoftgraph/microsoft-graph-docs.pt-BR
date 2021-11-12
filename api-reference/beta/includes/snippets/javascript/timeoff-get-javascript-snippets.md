---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 229807c8ab1da5f446be508d0553656b1340bc473e860b2d91bd4a5f4476353b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100341"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let timeOff = await client.api('/teams/{teamId}/schedule/timesOff/{timeOffId}')
    .version('beta')
    .get();

```