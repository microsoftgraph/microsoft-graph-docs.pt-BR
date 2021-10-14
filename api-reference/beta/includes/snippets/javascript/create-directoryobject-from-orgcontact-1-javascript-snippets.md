---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b52e8655bc5a099ccef7e76e8c2a07ebece6cdbef960f82d55e6a72d1584e708
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159659"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  directoryObject: {
  }
};

await client.api('/contacts/{id}/directReports')
    .version('beta')
    .post(directoryObject);

```