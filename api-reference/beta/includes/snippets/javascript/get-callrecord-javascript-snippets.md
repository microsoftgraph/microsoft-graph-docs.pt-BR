---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 837dd51ca646a310500b070267a0d07a4f01d22c689a05a82ed2abfa7738f45d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101630"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let callRecord = await client.api('/communications/callRecords/{id}')
    .version('beta')
    .get();

```