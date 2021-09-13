---
title: Atualizar configurações
description: 'Atualize as propriedades do objeto de configurações. '
author: jpettere
ms.localizationpriority: medium
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 9da4b635c92f82e4983da164218013ac96009734
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59143913"
---
# <a name="update-settings"></a>Atualizar configurações

Namespace: microsoft.graph

Atualize as propriedades do [objeto userSettings.](../resources/usersettings.md) Os usuários na mesma organização podem ter configurações diferentes com base em suas preferências ou nas políticas da organização. Para obter as configurações atuais do usuário, consulte [configurações atuais do usuário](usersettings-get.md). 

### <a name="batch-request"></a>Solicitação em lote

Também é possível desativar vários usuários do Delve e desabilitar sua contribuição sobre a relevância do conteúdo para toda a organização por meio de uma solicitação em lotes.
Para saber mais, consulte [JSON batching](/graph/json-batching).

>**Importante:** somente membros do grupo de função [de gerenciamento](https://support.office.com/article/permissions-in-the-office-365-security-compliance-center-d10608af-7934-490a-818e-e68f17d0e9c1?ui=en-US&rs=en-US&ad=US) da organização podem atualizar vários usuários. 



## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | User.ReadWrite, User.ReadWrite.All   |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | User.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

```http
PATCH /me/settings
```

A solicitação com uma 'ID de usuário' ou 'userPrincipalName' só pode ser acessada pelo usuário ou por um usuário com as permissões User.ReadWrite.All. Para saber mais, consulte [Permissões](/graph/permissions-reference). 

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
|contributionToContentDiscoveryDisabled|Booliano|Definir como true desabilite o acesso de representante à API [de](/graph/api/resources/insights-trending?view=graph-rest-1.0) Tendência e desabilite o acesso aos documentos Office Delve para o usuário. A configuração como true também afeta a relevância do conteúdo exibido no Microsoft 365 - por exemplo, sites sugeridos no SharePoint Home e o exibição Descobrir no OneDrive for Business mostram resultados menos relevantes. Essa configuração reflete o estado de controle [em Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout).|

## <a name="example"></a>Exemplo 

##### <a name="request"></a>Solicitação

Aqui está um exemplo de solicitação sobre como desativar um usuário do Delve e desabilitar sua contribuição sobre a relevância do conteúdo para toda a organização.

```http
PATCH https://graph.microsoft.com/v1.0/me/settings
Content-type: application/json
Content-length: 37

{
  "contributionToContentDiscoveryDisabled": true
}
```

##### <a name="response"></a>Resposta

Aqui está um exemplo da resposta. Observação: o objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": true
}
```
