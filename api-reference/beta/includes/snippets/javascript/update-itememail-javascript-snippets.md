---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 87a262586f5edf38094e7a1f7149666f737485d3
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "37997349"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const itemEmail = {
  address: "address-value",
  displayName: "displayName-value",
  type: "type-value"
};

let res = await client.api('/me/profile/emails/{id}')
    .version('beta')
    .update(itemEmail);

```