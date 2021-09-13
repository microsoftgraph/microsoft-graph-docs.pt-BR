---
title: Obter mensagens do Outlook em uma pasta compartilhada ou delegada
description: O Outlook permite que os clientes compartilhem pastas de e-mail entre si e forneçam acesso de "leitura", "criação", "modificação" ou "exclusão" a pastas individuais. O Outlook também permite que um cliente representante a outro usuário agir em nome do cliente.
author: abheek-das
ms.localizationpriority: high
ms.prod: outlook
ms.openlocfilehash: c2798e01d29badc1d3228692d02caca1ab89fa87
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59071746"
---
# <a name="get-outlook-messages-in-a-shared-or-delegated-folder"></a>Obtenha mensagens do Outlook em uma pasta compartilhada ou delegada

O Outlook permite que os clientes compartilhem pastas de email entre si e forneçam acesso de "leitura", "criação", "modificação" ou "exclusão" a pastas individuais. O Outlook também permite que um cliente delegue outro usuário para agir em nome do cliente e acesse pastas de correio específicas ou toda a caixa de correio do cliente; isso também é conhecido como "delegação" no Outlook.

Programaticamente, o Microsoft Graph oferece suporte à obtenção de mensagens em pastas de email compartilhadas por outros usuários, bem como à obtenção das próprias pastas compartilhadas. O suporte também se aplica a pastas que foram delegadas.

Por exemplo, Garth compartilhou com John e deu acesso de leitura à caixa de entrada de Garth. Se John fez login em seu aplicativo e forneceu permissões delegadas (Mail.Read.Shared ou Mail.ReadWrite.Shared), seu aplicativo poderá acessar o email de Garth e a caixa de entrada de Garth conforme descrito abaixo.

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
