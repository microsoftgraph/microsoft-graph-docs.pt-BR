---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1f03a9b68c2fa2780899ee47697a404c5cdc38105fb7abda78ba469fba8d80e9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273295"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getrecentnotebooks = await client.api('/me/onenote/notebooks/getrecentnotebooks(includePersonalNotebooks=true)')
    .get();

```