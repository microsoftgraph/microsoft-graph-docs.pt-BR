---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a637700bbd9524083cfc618b4f0b51985cb7ef2f49aaca4d9a5c41e2d1ceaae5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101102"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let owners = await client.api('/applications/{id}/owners')
    .get();

```