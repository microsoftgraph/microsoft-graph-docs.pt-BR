---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b6f6f613a6e05ec718aed4908936096388374857e87104ee39e396a5bf35deac
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272734"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let channel = await client.api('/teams/{id}/primaryChannel')
    .get();

```