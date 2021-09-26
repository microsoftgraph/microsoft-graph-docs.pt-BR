---
author: nkramer
ms.topic: include
ms.date: 01/25/2021
ms.localizationpriority: medium
ms.openlocfilehash: 9a1c86904767b9cb9f36082d06733b36449fe920
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59763405"
---
<!-- markdownlint-disable MD041-->

### <a name="chatmessage"></a>chatMessage

**chatMessage** assinaturas com permissões delegadas não oferecem suporte a dados de recursos (**includeResourceData** deve ser `false`) e não requerem [criptografia](/graph/webhooks-with-resource-data). A única exceção é o recurso `/users/{id}/chats/getAllMessages` (disponível somente na versão beta) que oferece suporte a dados de recursos independentemente do tipo de permissão.

Assinaturas **chatMessage** com permissões de aplicativo incluem dados de recurso e exigem [criptografia](/graph/webhooks-with-resource-data). A criação de assinatura falhará se um [encryptionCertificate](/graph/api/resources/subscription) não for especificado. Antes de criar uma assinatura **chatMessage**, você deve solicitar acesso. Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).

> [!NOTE]
> `/teams/getAllMessages` e `/chats/getAllMessages` estão disponíveis para os usuários que possuem as [licenças necessárias](https://aka.ms/teams-changenotification-licenses). No futuro, a Microsoft poderá exigir que você ou seus clientes paguem taxas adicionais com base na quantidade de dados acessados através da API.
