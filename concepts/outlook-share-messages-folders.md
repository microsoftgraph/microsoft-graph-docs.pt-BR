---
title: Obter mensagens do Outlook em uma pasta compartilhada ou delegada
description: O Outlook permite que os clientes compartilhem pastas de e-mail entre si e forneçam acesso de "leitura", "criação", "modificação" ou "exclusão" a pastas individuais. O Outlook também permite que um cliente representante a outro usuário agir em nome do cliente.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 6de4ee7ca1ed179bc538bb7aa1f2a3dacb8adb80
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013440"
---
# <a name="get-outlook-messages-in-a-shared-or-delegated-folder"></a>Obtenha mensagens do Outlook em uma pasta compartilhada ou delegada

O Outlook permite que os clientes compartilhem pastas de email entre si e forneçam acesso de "leitura", "criação", "modificação" ou "exclusão" a pastas individuais. O Outlook também permite que um cliente delegue outro usuário para agir em nome do cliente e acesse pastas de correio específicas ou toda a caixa de correio do cliente; isso também é conhecido como "delegação" no Outlook.

O Microsoft Graph oferece suporte de forma programática para receber mensagens em pastas de email que foram compartilhadas por outros usuários, além de receber as pastas compartilhadas em si. O suporte também se aplica a pastas que foram delegadas.

Por exemplo, Henrique compartilhou com Diogo e deu a ele acesso de leitura à sua caixa de entrada. Se Diogo estiver conectado em seu aplicativo e tiver fornecido permissões delegadas (Mail.Read.Shared ou Mail.ReadWrite.Shared), o aplicativo poderá acessar o email e a caixa de entrada do Henrique conforme descrito abaixo.

## <a name="microsoft-graph-permissions"></a>Permissões do Microsoft Graph

Use as permissões delegadas, `Mail.Read.Shared` ou `Mail.ReadWrite.Shared`, para ler ou gravar mensagens em uma pasta compartilhada ou delegada. 

Observe que essas duas permissões não são [para se inscrever para alterar as notificações](webhooks.md) em itens em pastas compartilhadas ou delegadas. Para configurar assinaturas de notificação de alteração de mensagens em uma pasta de correio compartilhada, delegada, ou de qualquer outra pasta de correio de usuário no locatário, use a permissão do aplicativo,

Saiba mais em [permissões de correio](permissions-reference.md#mail-permissions).

## <a name="get-a-message-in-the-shared-folder"></a>Obtenha uma mensagem na pasta compartilhada

Você pode obter uma mensagem específica na caixa de entrada do Henrique:

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages/{id}
```

Após a conclusão bem-sucedida, você receberá HTTP 200 OK e a instância de [message](/graph/api/resources/message) identificada por `{id}` da caixa de entrada do Henrique.

## <a name="get-all-messages-in-the-shared-folder"></a>Obter todas as mensagens na pasta compartilhada

Obtenha todas as mensagens na caixa de entrada do Henrique:

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages
```

Após a conclusão bem-sucedida, você receberá HTTP 200 OK um conjunto de instâncias de [message](/graph/api/resources/message) na caixa de entrada do Henrique.

## <a name="get-the-shared-folder"></a>Obter a pasta compartilhada

Obtenha a pasta (caixa de entrada) que Henrique compartilhou com Diogo.

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')
```

Após a conclusão bem-sucedida, você receberá HTTP 200 OK e uma instância de [mailFolder](/graph/api/resources/mailfolder) que representa a pasta de caixa de entrada do Henrique.

Os mesmos recursos de GET se aplicam se Henrique delegar a Diogo mais acesso à sua caixa de entrada ou se Henrique delegar toda a sua caixa de correio a Diogo.

Se Henrique não tiver compartilhado sua caixa de entrada com Diogo nem delegado sua caixa de correio a Diogo, a especificação da ID de usuário de Henrique ou do nome de entidade de segurança nessas operações GET retornará um erro. 


## <a name="next-steps"></a>Próximas etapas

Saiba mais sobre:

- [Por que integrar-se com o email do Outlook](outlook-mail-concept-overview.md)
- [Como usar a API de email](/graph/api/resources/mail-api-overview) e seus [casos de uso](/graph/api/resources/mail-api-overview#common-use-cases) do Microsoft Graph versão 1.0.
