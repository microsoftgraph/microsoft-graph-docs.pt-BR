---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 737ab32ec43dd4d84cf37c978bfed82b0afd39ef
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35475644"
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