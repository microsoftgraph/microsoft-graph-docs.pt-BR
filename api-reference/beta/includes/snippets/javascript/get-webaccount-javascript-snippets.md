---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0474422695a980c2c1ea93432d473c9cbe232dc8
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37997462"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/profile/webAccounts/{id}')
    .version('beta')
    .get();

```