---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cfeecc060b711a0ca03046231c582c03a8e8a950
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50179530"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users')
    .header('ConsistencyLevel','eventual')
    .filter('endswith(mail,'a@contoso.com')')
    .orderby('userPrincipalName')
    .get();

```