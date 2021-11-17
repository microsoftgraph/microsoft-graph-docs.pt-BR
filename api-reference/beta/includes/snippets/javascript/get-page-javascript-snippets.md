---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4ea51b4127197691c1e896d49b2fc333d4e47e3796af2ca8a95127403383d6ec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899915"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let sitePage = await client.api('/sites/{site-id}/pages/{page-id}')
    .version('beta')
    .get();

```