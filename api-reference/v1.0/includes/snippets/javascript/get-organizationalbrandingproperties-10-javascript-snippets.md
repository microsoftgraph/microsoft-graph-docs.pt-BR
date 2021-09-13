---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a9122f609404432ce409b3349d623d3da89f1702c2cf6be8e127c51ae91dc51a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272405"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let string = await client.api('/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/en-US/signInPageText')
    .get();

```