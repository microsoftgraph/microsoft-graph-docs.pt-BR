---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2b6c4f4e63d5df03f1af1d2e5cb457b4e07cf5412a77a9863e5b5a588261849b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156340"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String clientContext = "d45324c1-fcb5-430a-902c-f20af696537c";

LinkedList<Prompt> promptsList = new LinkedList<Prompt>();
MediaPrompt prompts = new MediaPrompt();
MediaInfo mediaInfo = new MediaInfo();
mediaInfo.uri = "https://cdn.contoso.com/beep.wav";
mediaInfo.resourceId = "1D6DE2D4-CD51-4309-8DAA-70768651088E";
prompts.mediaInfo = mediaInfo;

promptsList.add(prompts);

Boolean loop = false;

graphClient.communications().calls("57dab8b1-894c-409a-b240-bd8beae78896")
    .playPrompt(CallPlayPromptParameterSet
        .newBuilder()
        .withPrompts(promptsList)
        .withLoop(loop)
        .withClientContext(clientContext)
        .build())
    .buildRequest()
    .post();

```