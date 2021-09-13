---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 68dd77b0b4fa55f7ebb2be97577afb0cb714d38ba117ccb7fc4e223c3ff4ee3c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57376783"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let automaticRepliesSetting = await client.api('/me/mailboxSettings/automaticRepliesSetting')
    .get();

```