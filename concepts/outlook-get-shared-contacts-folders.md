---
title: Obtenha os contatos do Outlook em uma pasta compartilhada
description: " Isso também é "
ms.openlocfilehash: c8c5b3a2eac49153826113af036146cc4475d9e5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091588"
---
# <a name="get-outlook-contacts-in-a-shared-folder"></a>Obtenha os contatos do Outlook em uma pasta compartilhada

Permite que os clientes do Outlook compartilhar pastas umas com as outras e forneça "ler", "criar", "modificar" ou "excluir" o acesso às pastas de contatos individuais. O Outlook também permite que um cliente delegar a outro usuário para agir em nome do cliente e pastas específicas de acesso ou caixa de correio inteira do cliente; Isso também é conhecida como "delegação" no Outlook.

Programaticamente, o Microsoft Graph suporta obtendo contatos em pastas de contatos que foram compartilhadas por outros usuários, bem como introdução às próprias pastas compartilhadas. O suporte também se aplica às pastas em uma caixa de correio delegada.

Por exemplo, Garth tem compartilhadas com John uma pasta de contato personalizada e oferecido acesso de leitura de John. Se John tiver entrado no seu aplicativo e oferecido permissões delegadas (Contacts.Read.Shared ou Contacts.ReadWrite.Shared), o seu aplicativo será capaz de acessar a pasta contato personalizada e os contatos nessa pasta, conforme descrito abaixo do Garth.

## <a name="get-a-contact-in-the-shared-folder"></a>Obtenha um contato na pasta compartilhada

Você pode obter um contato específico na pasta contato personalizada que Garth tiver compartilhado com John:

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts/{id}
```

Após a conclusão bem-sucedida, você obterá HTTP 200 Okey e a instância de [contato](/graph/api/resources/contact?view=graph-rest-1.0) identificado pela `{id}` da pasta compartilhada de contato do Garth.

## <a name="get-all-contacts-in-the-shared-folder"></a>Obtenha todos os contatos na pasta compartilhada

Obtenha todos os contatos na pasta compartilhada de contato do Garth:

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts
```

Após a conclusão bem-sucedida, você obterá HTTP 200 Okey e um conjunto de instâncias de [contato](/graph/api/resources/contact?view=graph-rest-1.0) do Garth compartilhado a pasta de contato.

## <a name="get-the-shared-folder"></a>Obter a pasta compartilhada

Obtenha a pasta de contato que Garth compartilhada com John.

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}
```

Após a conclusão bem-sucedida, você obterá HTTP 200 Okey e compartilhados de uma instância de [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-1.0) que representa Garth pasta de contato.

Os mesmos recursos GET aplicam se Garth tinha delegada John sua caixa de correio inteira.

Se Garth não compartilhou a pasta de contato com John, nem ele tem delegado sua caixa de correio de John, a especificação user ID do Garth ou o nome principal do usuário nessas operações GET retornará um erro. 


## <a name="next-steps"></a>Próximas etapas

Saiba mais sobre:

- [Por que integram com contatos pessoais do Outlook](outlook-contacts-concept-overview.md)
- Os [Contatos API](/graph/api/resources/contact?view=graph-rest-1.0) v 1.0 do Microsoft Graph.