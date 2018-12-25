---
title: Obter mensagens do Outlook em uma pasta compartilhada ou delegada
description: O Outlook permite que os clientes compartilhem pastas de e-mail entre si e forneçam acesso de "leitura", "criação", "modificação" ou "exclusão" a pastas individuais. O Outlook também permite que um cliente representante a outro usuário agir em nome do cliente.
author: angelgolfer-ms
ms.openlocfilehash: cdb2228c64647497674402825577942323c3d2ff
ms.sourcegitcommit: 8feddb85e436be5581557a199f2e46d5b4ebfa21
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/22/2018
ms.locfileid: "27413173"
---
# <a name="get-outlook-messages-in-a-shared-or-delegated-folder"></a>Obtenha mensagens do Outlook em uma pasta compartilhada ou delegada

O Outlook permite que os clientes compartilhem pastas de email entre si e forneçam acesso de "leitura", "criação", "modificação" ou "exclusão" a pastas individuais. O Outlook também permite que um cliente delegue outro usuário para agir em nome do cliente e acesse pastas de correio específicas ou toda a caixa de correio do cliente; isso também é conhecido como "delegação" no Outlook.

O Microsoft Graph oferece suporte de forma programática para receber mensagens em pastas de email que foram compartilhadas por outros usuários, além de receber as pastas compartilhadas em si. O suporte também se aplica a pastas que foram delegadas.

Por exemplo, Henrique compartilhou com Diogo e deu a ele acesso de leitura à sua caixa de entrada. Se Diogo estiver conectado em seu aplicativo e tiver fornecido permissões delegadas (Mail.Read.Shared ou Mail.ReadWrite.Shared), o aplicativo poderá acessar o email e a caixa de entrada do Henrique conforme descrito abaixo.

> **Observação** permissões de compartilhamento (Mail.Read.Shared ou Mail.ReadWrite.Shared) permitem a você ler ou escrever mensagens em uma pasta compartilhada ou delegada. Eles não têm suporte [subscrever alterar notificações](webhooks.md) em pastas como essas. Para configurar as assinaturas de notificação de alteração em mensagens na pasta de e-mail compartilhado, representante ou qualquer outra de um usuário no locatário, use a permissão de aplicativo Mail.Read.

## <a name="get-a-message-in-the-shared-folder"></a>Obtenha uma mensagem na pasta compartilhada

Você pode obter uma mensagem específica na caixa de entrada do Henrique:

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages/{id}
```

Após a conclusão bem-sucedida, você receberá HTTP 200 OK e a instância de [message](/graph/api/resources/message?view=graph-rest-1.0) identificada por `{id}` da caixa de entrada do Henrique.

## <a name="get-all-messages-in-the-shared-folder"></a>Obter todas as mensagens na pasta compartilhada

Obtenha todas as mensagens na caixa de entrada do Henrique:

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages
```

Após a conclusão bem-sucedida, você receberá HTTP 200 OK um conjunto de instâncias de [message](/graph/api/resources/message?view=graph-rest-1.0) na caixa de entrada do Henrique.

## <a name="get-the-shared-folder"></a>Obter a pasta compartilhada

Obtenha a pasta (caixa de entrada) que Henrique compartilhou com Diogo.

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')
```

Após a conclusão bem-sucedida, você receberá HTTP 200 OK e uma instância de [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0) que representa a pasta de caixa de entrada do Henrique.

Os mesmos recursos de GET se aplicam se Henrique delegar a Diogo mais acesso à sua caixa de entrada ou se Henrique delegar toda a sua caixa de correio a Diogo.

Se Henrique não tiver compartilhado sua caixa de entrada com Diogo nem delegado sua caixa de correio a Diogo, a especificação da ID de usuário de Henrique ou do nome de entidade de segurança nessas operações GET retornará um erro. 


## <a name="next-steps"></a>Próximas etapas

Saiba mais sobre:

- [Por que integrar-se com o email do Outlook](outlook-mail-concept-overview.md)
- [Como usar a API de email](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) e seus [casos de uso](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases) do Microsoft Graph versão 1.0.