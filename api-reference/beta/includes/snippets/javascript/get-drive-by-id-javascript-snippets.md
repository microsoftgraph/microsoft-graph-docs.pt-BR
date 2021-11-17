---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1085eed6a6dc5817537d5f8ae0e05a01f08318ff75e07b0e576c449e982f95cc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100883"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let drive = await client.api('/drives/{driveId}')
    .version('beta')
    .get();

```