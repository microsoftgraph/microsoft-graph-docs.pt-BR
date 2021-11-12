---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: abcdb0c75793db6e92f688f2e7beea94b00207192b65ca292b5426cfce39859c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157134"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/print/shares/{printerShareId}')
    .delete();

```