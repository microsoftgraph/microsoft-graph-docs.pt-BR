---
title: Receber mensagens do Outlook em uma pasta compartilhada ou delegada
description: Esses tópicos também têm a seção semelhante - listar eventos, obtenha o evento, obtenha o calendário, lista de contatos, fazer contato, obter pasta de contato.
ms.openlocfilehash: d9e04527879cb32f14dc8d74a814a54150c5b2d0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091638"
---
# <a name="get-outlook-messages-in-a-shared-or-delegated-folder"></a>Receber mensagens do Outlook em uma pasta compartilhada ou delegada

<!-- remove similar content in other topics when ready to publish - list messages, get message, get mail folder.
These topics also have similar section - list events, get event, get calendar, list contacts, get contact, get contact folder.
-->

Permite que os clientes do Outlook compartilhar pastas de email umas com as outras e forneça "ler", "criar", "modificar" ou "excluir" o acesso às pastas individuais. O Outlook também permite que um cliente delegar a outro usuário para agir em nome do cliente e acessar pastas de email específico ou caixa de correio inteira do cliente; Isso também é conhecida como "delegação" no Outlook.

O Microsoft Graph oferece suporte de forma programática para receber mensagens em pastas de email que foram compartilhadas por outros usuários, além de receber as pastas compartilhadas em si. O suporte também se aplica às pastas que foram delegadas.

Por exemplo, Garth tem compartilhadas com John e oferecido acesso de leitura à caixa de entrada do Garth. Se John tiver entrado no seu aplicativo e oferecido permissões delegadas (Mail.Read.Shared ou Mail.ReadWrite.Shared), o seu aplicativo será capaz de acessar o email do Garth e caixa de entrada do Garth conforme descrito abaixo.

## <a name="get-a-message-in-the-shared-folder"></a>Obter uma mensagem na pasta compartilhada

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

Se Garth não tiver compartilhado sua caixa de entrada com John, nem ele tem delegado sua caixa de correio de John, a especificação user ID do Garth ou o nome principal do usuário nessas operações GET retornará um erro. 


## <a name="next-steps"></a>Próximas etapas

Saiba mais sobre:

- [Por que integrar-se com o email do Outlook](outlook-mail-concept-overview.md)
- [Como usar a API de email](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) e seus [casos de uso](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases) do Microsoft Graph versão 1.0.