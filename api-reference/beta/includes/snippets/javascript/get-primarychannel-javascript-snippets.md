---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e879061ea0df237e2e740aa714c747b8c5ab14c66aa3bf2d23873789b40d2d0c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156897"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let channel = await client.api('/teams/{id}/primaryChannel')
    .version('beta')
    .get();

```