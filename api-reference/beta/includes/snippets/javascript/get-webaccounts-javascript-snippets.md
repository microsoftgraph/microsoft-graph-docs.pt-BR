---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a6893032250a3876e263cc3e25811ef566f650b1
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37996835"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/profile/webAccounts')
    .version('beta')
    .get();

```