---
author: nkramer
ms.topic: include
ms.date: 01/25/2021
ms.author: nkramer
ms.openlocfilehash: ef6cf05f93a8a7f33926ba253e9241bb4c445ad1
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034070"
---
<!-- markdownlint-disable MD041-->

### <a name="chatmessage"></a>chatMessage

**chatMessage** assinaturas com permissões delegadas não oferecem suporte a dados de recursos (**includeResourceData** deve ser `false`) e não requerem [criptografia](/graph/webhooks-with-resource-data).

Assinaturas **chatMessage** com permissões de aplicativo incluem dados de recurso e exigem [criptografia](/graph/webhooks-with-resource-data). A criação da assinatura falhará se [encryptionCertificate](/graph/api/resources/subscription) não for especificado. Antes de criar uma assinatura **chatMessage**, você deve solicitar acesso. Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis). 

> **Observações:** 
>
>`/teams/getAllMessages` e `/chats/getAllMessages` estão disponíveis para usuários que possuem as [licenças necessárias](https://aka.ms/teams-changenotification-licenses).
No futuro, a Microsoft poderá exigir que você ou seus clientes paguem taxas adicionais com base na quantidade de dados acessados pela API.
>
>`/chats/getAllMessages` retorna apenas mensagens de bate-papos pertencentes ao locatário. Se um thread de bate papo for iniciado por um usuário fora do locatário, esse thread de bate papo não será de propriedade do locatário e não criará notificações de alteração.
