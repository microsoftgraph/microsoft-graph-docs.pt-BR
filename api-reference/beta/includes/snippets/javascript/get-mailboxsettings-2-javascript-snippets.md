---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 737ab32ec43dd4d84cf37c978bfed82b0afd39ef
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724278"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailboxSettings/automaticRepliesSetting')
    .version('beta')
    .get();

```