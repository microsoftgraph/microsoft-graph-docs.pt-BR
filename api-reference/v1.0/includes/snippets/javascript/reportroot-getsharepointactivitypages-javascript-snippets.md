---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f6522b6e897e9d55798349b478bfc08bed3a7051
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740685"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSharePointActivityPages(period='D7')')
    .get();

```