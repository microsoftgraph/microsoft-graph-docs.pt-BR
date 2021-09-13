---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ba3f7b16355e7b6a982e8ea25d6aba2042889bbd718d8839a1e613163053df0f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272183"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let supportedLanguages = await client.api('/me/outlook/supportedLanguages')
    .get();

```