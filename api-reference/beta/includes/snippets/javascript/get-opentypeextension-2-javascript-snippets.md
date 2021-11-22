---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 625377ec43ea27357aae0fa9fbbf664683d4d624347ffaf03eba33d90687655a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213779"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let extension = await client.api('/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVl17IsAAA=/extensions/Com.Contoso.Deal')
    .version('beta')
    .get();

```