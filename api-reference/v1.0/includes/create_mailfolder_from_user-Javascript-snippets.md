---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cf73b72bfb1628f6a9ff1249a66f986edc6c31b4
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34460507"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailFolder = {
  displayName: "displayName-value"
};

let res = await client.api('/me/mailFolders')
    .post({mailFolder : mailFolder});

```