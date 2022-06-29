---
title: Obter contatos do Outlook em uma pasta compartilhada
description: No Outlook, os clientes podem compartilhar pastas de contatos e fornecer acesso a pastas. O Outlook também permite que um cliente delegue outro usuário para agir em nome do cliente.
author: angelgolfer-ms
ms.localizationpriority: medium
ms.prod: outlook
ms.openlocfilehash: 7be7fb4ddf0d91b74c936b01df4e6bfbdd02ee44
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66444352"
---
# <a name="get-outlook-contacts-in-a-shared-folder"></a>Obter contatos do Outlook em uma pasta compartilhada

O Outlook permite que os clientes compartilhem pastas entre si e forneçam acesso de "leitura", "criação", "modificação" ou "exclusão" a pastas de contatos individuais. O Outlook também permite que um cliente delegue outro usuário para agir em nome do cliente e acesse pastas específicas ou toda a caixa de correio do cliente; isso também é conhecido como *delegação* no Outlook.

O Microsoft Graph oferece suporte de forma programática à obtenção de contatos em pastas de contatos que foram compartilhadas por outros usuários, além de receber as pastas compartilhadas em si. O suporte também se aplica a pastas em uma caixa de correio delegada.

Por exemplo, Henrique compartilhou com Diogo uma pasta de contatos personalizada e deu a ele acesso de leitura. Se João tiver entrado em seu aplicativo e fornecido permissões delegadas (Contacts.Read.Shared ou Contacts.ReadWrite.Shared), seu aplicativo poderá acessar a pasta de contatos personalizada de Henrique e os contatos nessa pasta. Para obter detalhes, consulte as seções a seguir.

> [!NOTE]
> As permissões de compartilhamento (Contacts.Read.Shared ou Contacts.ReadWrite.Shared) permitem que você leia ou grave contatos em uma pasta compartilhada ou delegada. Eles não têm suporte [subscrever alterar notificações](webhooks.md) em itens nessas pastas. Para configurar as assinaturas de notificação de alteração nos contatos na pasta de contatos compartilhada, representante ou qualquer outra de um usuário no locatário, use a permissão de aplicativo Contacts.Read.

## <a name="get-a-contact-in-the-shared-folder"></a>Obter um contato na pasta compartilhada

Você pode obter um contato específico na pasta de contatos personalizada que Henrique compartilhou com Diogo:

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts/{id}
```

Após a conclusão bem-sucedida, você receberá HTTP 200 OK e a instância de [contact](/graph/api/resources/contact) identificada por `{id}` da pasta de contatos compartilhada de Henrique.

## <a name="get-all-contacts-in-the-shared-folder"></a>Obter todos os contatos na pasta compartilhada

Obtenha todos os contatos na pasta de contatos compartilhada do Henrique:

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts
```

Após a conclusão bem-sucedida, você receberá HTTP 200 OK e uma coleção de instâncias de [contact](/graph/api/resources/contact) na pasta de contatos compartilhada de Henrique.

## <a name="get-the-shared-folder"></a>Obter a pasta compartilhada

Obtenha a pasta de contatos que Henrique compartilhou com Diogo.

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}
```

Após a conclusão bem-sucedida, você receberá HTTP 200 OK e uma instância de [contactFolder](/graph/api/resources/contactfolder) que representa a pasta de contatos compartilhada de Henrique.

As mesmas funcionalidades GET se aplicariam se Henrique tivesse delegado a Diogo toda a sua caixa de correio.

Se Henrique não tiver compartilhado sua pasta de contatos com Diogo nem delegado sua caixa de correio a Diogo, a especificação da ID de usuário de Henrique ou do nome UPN nessas operações GET retornará um erro. 


## <a name="next-steps"></a>Próximas etapas

Saiba mais sobre:

- [Por que se integrar aos contatos pessoais do Outlook](outlook-contacts-concept-overview.md)
- A [API de contatos](/graph/api/resources/contact) do Outlook no Microsoft Graph v1.0.
