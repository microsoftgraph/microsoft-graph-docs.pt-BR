---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 123cb7673d5d7767be5859dfc89a6fa773fa952b43946a893042398bd79ac819
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102768"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let messages = await client.api('/me/mailFolders/{id}/messages')
    .get();

```