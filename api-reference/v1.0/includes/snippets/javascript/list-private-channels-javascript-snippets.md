---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aa74332b562ded029cb98cc2c16f69b2c6d035f2
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/07/2020
ms.locfileid: "48373592"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/channels')
    .version('beta')
    .filter('membershipType eq 'private'')
    .get();

```