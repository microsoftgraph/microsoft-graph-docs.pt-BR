---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ff985df9e0675858063493672c3091e4530eebf9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740721"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailFolders/inbox/messageRules/AQAAAJ5dZqA=')
    .get();

```