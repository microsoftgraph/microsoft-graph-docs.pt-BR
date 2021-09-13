---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cb00070a588d3d482747053bc84389b64e912c980c507ce370fe80fe25286765
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100011"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/calendarGroups/{id}')
    .delete();

```