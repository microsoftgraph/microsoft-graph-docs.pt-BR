---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d50b46fb25590b0632acdf829135a19d277c774ee9dbfd6c39e5a387b6e60460
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275379"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/applications/{id}/owners/{id}/$ref')
    .delete();

```