---
title: Atualizar AuthorizationPolicy
description: Atualize as propriedades do objeto authorizationPolicy.
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ac605e93603cb39491fd980e78a9b0f0026541eb
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2020
ms.locfileid: "44492194"
---
# <a name="update-authorizationpolicy"></a>Atualizar authorizationPolicy

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualiza as propriedades de um objeto [authorizationPolicy](../resources/authorizationpolicy.md) .

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Policy. ReadWrite. Authorization|
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Policy. ReadWrite. Authorization|

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/authorizationPolicy/authorizationPolicy
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Descrição|
|:-----------|:-----------|
| Autorização | Portador {token} |
| Content-type | application/json |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|  
|displayName|Cadeia de caracteres| Nome para exibição dessa política. |  
|description|String| Descrição da política. |  
|guestUserRoleId|Guid| Representa o modelo de função para a função que deve ser concedida ao usuário convidado. Consulte [list unifiedRoleDefinitions](https://docs.microsoft.com/graph/api/rbacapplication-list-roledefinitions?view=graph-rest-beta&tabs=http) para encontrar a lista de modelos de função disponíveis. Somente as funções suportadas hoje são usuário (a0b1b346-4d3e-4e8b-98f8-753987be4970), usuário convidado (10dae51f-b6af-4016-8d66-8c2a99b929b3) e usuário convidado restrito (2af84b1e-32c8-42b7-82bc-daa82404023b). | 
|enabledPreviewFeatures|Coleção (cadeia de caracteres)| Lista de recursos habilitados para visualização privada no locatário. | 
|blockMsolPowerShell|Booliano| Para desabilitar o uso do MSOL PowerShell, defina essa propriedade como `true` . A configuração `true` também desabilitará o acesso baseado no usuário ao ponto de extremidade de serviço herdado usado pelo MSol PowerShell. Isso não afeta o Azure AD Connect ou o Microsoft Graph. | 

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="example-1-update-or-set-guest-user-access-level-for-the-tenant"></a>Exemplo 1: atualizar ou definir o nível de acesso do usuário convidado para o locatário

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação. Neste exemplo, o nível de acesso de convidado é modificado para o usuário convidado restrito.

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy
{
  "guestUserRole": "2af84b1e-32c8-42b7-82bc-daa82404023b"
}

```
#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content

```

### <a name="example-2-enable-new-feature-for-preview-on-tenant"></a>Exemplo 2: habilitar novo recurso para visualização no locatário

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy
{
  "enabledPreviewFeatures": ["assignGroupsToRoles"]
}

```
#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content
```


### <a name="example-3-block-msol-powershell-in-tenant"></a>Exemplo 3: bloquear o MSOL PowerShell no locatário

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy
{
  "blockMsolPowerShell": true
}

```
#### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content
```
