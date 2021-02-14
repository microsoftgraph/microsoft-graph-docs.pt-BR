---
author: nkramer
ms.topic: include
ms.date: 01/25/2021
ms.openlocfilehash: f2def5f5a22267146d5b3005cd2f9be82e1d0db9
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50243118"
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
