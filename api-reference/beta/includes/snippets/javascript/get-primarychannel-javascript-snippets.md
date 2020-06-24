---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fcb2751781f813c2dbbe814bd9f6204268844020
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863445"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/primaryChannel')
    .version('beta')
    .get();

```