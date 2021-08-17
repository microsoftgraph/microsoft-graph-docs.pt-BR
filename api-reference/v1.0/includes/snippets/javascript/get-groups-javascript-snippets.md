---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a62bbc601fa97d74570e6d9dbd03c61456aa06a37daad4ad2af6631689ad1257
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215264"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let groups = await client.api('/groups')
    .get();

```