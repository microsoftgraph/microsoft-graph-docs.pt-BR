---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 38890f915072d4ef6abbd30d026dea57ae81f3c618de6acb50da2bf70a874bdf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217576"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let agreementAcceptances = await client.api('/me/agreementAcceptances')
    .version('beta')
    .get();

```