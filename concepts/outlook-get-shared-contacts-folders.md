---
title: Obter contatos do Outlook em uma pasta compartilhada
description: O Outlook permite que os clientes compartilhem pastas entre si e forneçam acesso de "leitura", "criação", "modificação" ou "exclusão" a pastas de contatos individuais. O Outlook também permite que um cliente representante a outro usuário agir em nome do cliente.
author: angelgolfer-ms
ms.localizationpriority: medium
ms.prod: outlook
ms.openlocfilehash: 3c1673dd6b551d1626187ee120ccc5e08550933b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59135925"
---
# <a name="get-outlook-contacts-in-a-shared-folder"></a>Obter contatos do Outlook em uma pasta compartilhada

O Outlook permite que os clientes compartilhem pastas entre si e forneçam acesso de "leitura", "criação", "modificação" ou "exclusão" a pastas de contatos individuais. O Outlook também permite que um cliente delegue outro usuário para agir em nome do cliente e acesse pastas específicas ou toda a caixa de correio do cliente; isso também é conhecido como "delegação" no Outlook.

O Microsoft Graph oferece suporte de forma programática à obtenção de contatos em pastas de contatos que foram compartilhadas por outros usuários, além de receber as pastas compartilhadas em si. O suporte também se aplica a pastas em uma caixa de correio delegada.

Por exemplo, Henrique compartilhou com Diogo uma pasta de contatos personalizada e deu a ele acesso de leitura. Se Diogo se conectou ao seu aplicativo e forneceu permissões delegadas (Contacts.Read.Shared ou Contacts.ReadWrite.Shared), o aplicativo poderá acessar a pasta de contatos personalizada de Henrique e os contatos nessa pasta, conforme descrito abaixo.

> **Observação** permissões de compartilhamento (Contacts.Read.Shared ou Contacts.ReadWrite.Shared) permitem que a você ler ou escrever contatos em uma pasta compartilhada ou delegada. Eles não têm suporte [subscrever alterar notificações](webhooks.md) em itens nessas pastas. Para configurar as assinaturas de notificação de alteração nos contatos na pasta de contatos compartilhada, representante ou qualquer outra de um usuário no locatário, use a permissão de aplicativo Contacts.Read.

## <a name="get-a-contact-in-the-shared-folder"></a>Obter um contato na pasta compartilhada

Você pode obter um contato específico na pasta de contatos personalizada que Henrique compartilhou com Diogo:

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts/{id}
```

Após a conclusão bem-sucedida, você receberá HTTP 200 OK e a instância de [contact](/graph/api/resources/contact?view=graph-rest-1.0) identificada por `{id}` da pasta de contatos compartilhada de Henrique.

## <a name="get-all-contacts-in-the-shared-folder"></a>Obter todos os contatos na pasta compartilhada

Obtenha todos os contatos na pasta de contatos compartilhada do Henrique:

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts
```

Após a conclusão bem-sucedida, você receberá HTTP 200 OK e uma coleção de instâncias de [contact](/graph/api/resources/contact?view=graph-rest-1.0) na pasta de contatos compartilhada de Henrique.

## <a name="get-the-shared-folder"></a>Obter a pasta compartilhada

Obtenha a pasta de contatos que Henrique compartilhou com Diogo.

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}
```

Após a conclusão bem-sucedida, você receberá HTTP 200 OK e uma instância de [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-1.0) que representa a pasta de contatos compartilhada de Henrique.

As mesmas funcionalidades GET se aplicariam se Henrique tivesse delegado a Diogo toda a sua caixa de correio.

Se Henrique não tiver compartilhado sua pasta de contatos com Diogo nem delegado sua caixa de correio a Diogo, a especificação da ID de usuário de Henrique ou do nome UPN nessas operações GET retornará um erro. 


## <a name="next-steps"></a>Próximas etapas

Saiba mais sobre:

- [Por que se integrar aos contatos pessoais do Outlook](outlook-contacts-concept-overview.md)
- A [API de contatos](/graph/api/resources/contact?view=graph-rest-1.0) do Outlook no Microsoft Graph v1.0.
