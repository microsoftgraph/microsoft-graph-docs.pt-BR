---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dbdca17511e8b2bca5c4cc69825f8db8e1dd7595
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35722332"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getYammerGroupsActivityDetail(period='D7')')
    .get();

```