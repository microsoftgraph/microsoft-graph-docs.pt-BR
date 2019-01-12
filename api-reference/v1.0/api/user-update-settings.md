---
title: Configurações de atualização
description: 'Atualize as propriedades do objeto de configurações. '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: be8ed27ecff80017cab56e1d3d20755cf68351cc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980269"
---
# <a name="update-settings"></a>Configurações de atualização

Atualize as propriedades do objeto de [configurações](../resources/user-settings.md) . Os usuários na mesma organização podem ter configurações diferentes com base em suas preferências ou nas diretivas de organização. Para obter as configurações atuais de usuário, consulte [configurações do usuário atual](user-get-settings.md). 

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | User.ReadWrite, User.ReadWrite.All   |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | User.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

```http
PATCH https://graph.microsoft.com/v1.0/me/settings
```

Solicitar com uma id de usuário' ' ou 'userPrincipalName' só está acessível pelo usuário ou por um usuário com as permissões User.ReadWrite.All. Para saber mais, consulte [Permissions](/graph/permissions-reference). 

```http
PATCH https://graph.microsoft.com/v1.0/users/{id | userPrincipalName}/settings/
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
|contributionToContentDiscoveryDisabled|Booliano|Definido como verdadeiro desabilitar o acesso de representante a [tendência](/graph/api/resources/insights-trending?view=graph-rest-beta) API e para desabilitar o acesso a documentos do Office me aprofundar para o usuário. Configuração como true também afeta a relevância do conteúdo exibido no Office 365 - por exemplo, sites sugeridos na página inicial do SharePoint e o modo de descoberta no OneDrive for Business mostram resultados menos relevantes. Essa configuração reflete o estado de controle no [Office me aprofundar](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).|

## <a name="example"></a>Exemplo 

##### <a name="request"></a>Solicitação

Aqui está um exemplo de solicitação sobre como um usuário da Delve recusar e desabilitar a sua contribuição sobre relevância de conteúdo para a organização inteira.

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

Também é possível sair vários usuários do Delve e desabilitar pela sua contribuição sobre relevância de conteúdo para toda a organização por meio de uma solicitação de lote.
Para saber mais, consulte [JSON processamento em lotes](https://developer.microsoft.com/graph/docs/concepts/json_batching).

**Importante**: somente membros do grupo de funções de [Gerenciamento da organização](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US) podem atualizar vários usuários. 



