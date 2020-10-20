---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ce5619fa6d8ca2bc1d61a8a58ed9d4cb9a8616fb
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48621166"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/threads/AAQkADJizZJpEWwqDHsEpV_KA==/posts/AAMkADJiUg96QZUkA-ICwMubAADDEd7UAAA=/extensions/Microsoft.OutlookServices.OpenTypeExtension.Com.Contoso.Estimate')
    .version('beta')
    .get();

```