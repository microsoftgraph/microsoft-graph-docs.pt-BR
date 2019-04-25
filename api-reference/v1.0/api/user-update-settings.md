---
title: Atualizar configurações
description: 'Atualize as propriedades do objeto Settings. '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: eb739ebe4266dc61246fd39f1b4f053ab08a5a75
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573568"
---
# <a name="update-settings"></a>Atualizar configurações

Atualize as propriedades do objeto [Settings](../resources/user-settings.md) . Os usuários na mesma organização podem ter configurações diferentes com base em suas preferências ou nas políticas da organização. Para obter as configurações atuais do usuário, confira [configurações atuais do usuário](user-get-settings.md). 

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | User. ReadWrite, User. ReadWrite. All   |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | User.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

```http
PATCH /me/settings
```

A solicitação com uma "ID de usuário" ou "userPrincipalName" só pode ser acessada pelo usuário ou por um usuário com as permissões User. ReadWrite. All. Para saber mais, confira [permissões](/graph/permissions-reference). 

```http
PATCH /users/{id | userPrincipalName}/settings/
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Cabeçalho       | Valor|
|:-----------|:------|
| Autorização  | {token} de portador. Obrigatório.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|contributionToContentDiscoveryDisabled|Booliano|Defina como true para desabilitar o acesso de representante à API de [tendências](/graph/api/resources/insights-trending?view=graph-rest-beta) e desabilitar o acesso aos documentos no Office Delve para o usuário. A configuração como true também afeta a relevância do conteúdo exibido no Office 365-por exemplo, sites sugeridos na página inicial do SharePoint e o modo de exibição de descoberta no OneDrive for Business mostrar resultados menos relevantes. Essa configuração reflete o estado de controle no [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).|

## <a name="example"></a>Exemplo 

##### <a name="request"></a>Solicitação

Veja a seguir um exemplo de solicitação de como recusar um usuário de aprofundar e desabilitar sua contribuição na relevância do conteúdo para toda a organização.

```http
PATCH https://graph.microsoft.com/v1.0/me/settings
Content-type: application/json
Content-length: 37

{
  "contributionToContentDiscoveryDisabled": true
}
```

##### <a name="response"></a>Resposta

Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": true
}
```

#### <a name="batch-request"></a>Solicitação em lote

Também é possível recusar vários usuários do Delve e desabilitar sua contribuição na relevância do conteúdo para toda a organização por meio de uma solicitação em lote.
Para saber mais, confira [batchIng JSON](https://developer.microsoft.com/graph/docs/concepts/json_batching).

**Importante**: somente os membros do grupo de função [Gerenciamento da organização](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US) podem atualizar vários usuários. 



