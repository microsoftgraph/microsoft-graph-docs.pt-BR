---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 764e3a413f4a1a19b86700b11f8118ea99f2cfe5649d0a67263fb4d27b18c438
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156646"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let services = await client.api('/print/services')
    .get();

```