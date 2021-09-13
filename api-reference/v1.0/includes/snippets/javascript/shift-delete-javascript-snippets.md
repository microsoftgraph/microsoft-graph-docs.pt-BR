---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a0717c141cb71a31978f7f95096fd01c422335801afe91a8a3e6595709e500d1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56900277"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/{teamId}/schedule/shifts/{shiftId}')
    .delete();

```