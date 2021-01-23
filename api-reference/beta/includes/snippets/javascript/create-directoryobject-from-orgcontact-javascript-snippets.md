---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6111db12148041fa5b6e327f56cadb9205c99281
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49946257"
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

let res = await client.api('/contacts/{id}/directReports')
    .version('beta')
    .post(directoryObject);

```