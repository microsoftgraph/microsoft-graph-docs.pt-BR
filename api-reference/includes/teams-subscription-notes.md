---
author: nkramer
ms.topic: include
ms.date: 01/25/2021
ms.localizationpriority: medium
ms.openlocfilehash: 398ba544748b3bf60728eda051059fc6f7e1d517
ms.sourcegitcommit: 94dc71a6d4fbdc46f2681a1add13416bc9b4a6e9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/05/2021
ms.locfileid: "60115163"
---
<!-- markdownlint-disable MD041-->

### <a name="chatmessage"></a>chatMessage

**chatMessage** assinaturas com permissões delegadas não oferecem suporte a dados de recursos (**includeResourceData** deve ser `false`) e não requerem [criptografia](/graph/webhooks-with-resource-data). A única exceção é o recurso `/users/{id}/chats/getAllMessages` (disponível somente na versão beta) que oferece suporte a dados de recursos independentemente do tipo de permissão.

Assinaturas **chatMessage** com permissões de aplicativo incluem dados de recurso e exigem [criptografia](/graph/webhooks-with-resource-data). A criação de assinatura falhará se um [encryptionCertificate](/graph/api/resources/subscription) não for especificado. Antes de criar uma assinatura **chatMessage**, você deve solicitar acesso. Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).

> [!NOTE]
>`/teams/getAllMessages`e `/chats/getAllMessages` tem [requisitos de licenciamento e pagamento.](/graph/teams-licenses)
> `/teams/getAllMessages` e `/chats/getAllMessages` dar suporte a `model=A` `model=B` parâmetros de consulta e.
> Se nenhum modelo for especificado, o [modo de avaliação](/graph/teams-licenses#evaluation-mode-default-requirements) será usado.

### <a name="conversationmember"></a>conversationMember

> [!NOTE]
>`/teams/getAllMembers`e `/chats/getAllMembers` tem [requisitos de licenciamento e pagamento.](/graph/teams-licenses)
> `/teams/getAllMembers` e `/chats/getAllMembers` dar suporte a `model=A` `model=B` parâmetros de consulta e.
> Se nenhum modelo for especificado, o [modo de avaliação](/graph/teams-licenses#evaluation-mode-default-requirements) será usado.