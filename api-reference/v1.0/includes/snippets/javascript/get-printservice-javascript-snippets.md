---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fbad5ecc6bfe99d56e917f59ae1e5e565692e8d3dc3d2fcca9173b3c0e4a8983
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214000"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printService = await client.api('/print/services/{printServiceId}')
    .get();

```