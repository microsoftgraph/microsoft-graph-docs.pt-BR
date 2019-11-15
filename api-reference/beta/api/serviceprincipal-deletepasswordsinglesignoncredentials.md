---
title: 'servicePrincipalName: deletePasswordSingleSignOnCredentials'
description: Exclua as credenciais de logon único usando uma senha para um usuário ou grupo.
localization_priority: Normal
author: bharathramh92
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9b39bf30f4a6a943a21db012d0201812681dd9ee
ms.sourcegitcommit: ef8eac3cf973a1971f8f1d41d75a085fad3690f0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/15/2019
ms.locfileid: "38658818"
---
# <a name="serviceprincipal-deletepasswordsinglesignoncredentials"></a>servicePrincipalName: deletePasswordSingleSignOnCredentials

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Exclua as credenciais de logon único usando uma senha para um usuário ou grupo.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Application. ReadWrite. All (também precisa Directory. Read. All), Directory. AccessAsUser. All, Directory. ReadWrite. All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Application. ReadWrite. All (também precisa Directory. Read. All), Directory. ReadWrite. All |

> [!NOTE]
> Os usuários podem criar credenciais para si mesmos. Os proprietários e administradores da entidade de serviço com as seguintes funções podem criar credenciais para qualquer usuário ou grupo: GlobalAdministrator, ApplicationAdministrator, CloudApplicationAdministrator. Para saber mais, confira [funções de diretório](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles).

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/deletePasswordSingleSignOnCredentials
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição   |
|:--------------|:--------------|
| Autorização | {token} de portador. Obrigatório. |
| Content-Type  | application/json. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação

Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro    | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|String|A ID do usuário ou grupo ao qual esse conjunto de credenciais pertence.|

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_deletepasswordsinglesignoncredentials"
}-->

```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/deletePasswordSingleSignOnCredentials
Content-type: application/json

{
  "id": "5793aa3b-cca9-4794-679a240f8b58"
}
```

### <a name="response"></a>Resposta

Este é um exemplo de resposta.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePrincipal: deletePasswordSingleSignOnCredentials",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
