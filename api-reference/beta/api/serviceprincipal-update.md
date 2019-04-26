---
title: Atualizar o servicePrincipalName
description: Atualiza as propriedades do objeto servicePrincipalName.
localization_priority: Normal
ms.openlocfilehash: 9bb3f8b578d3a0e24418f80da693ff317a7cc132
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33331433"
---
# <a name="update-serviceprincipal"></a>Atualizar o servicePrincipalName

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualiza as propriedades do objeto servicePrincipalName.
## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Directory.AccessAsUser.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Application.ReadWrite.OwnedBy, Application.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PATCH /servicePrincipals/{id}
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição|
|:-----------|:------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|accountEnabled|Booliano|                **True** se a entidade de serviço estiver habilitada; caso contrário, **false**.            |
|appDisplayName|Cadeia de caracteres|O nome de exibição exposto pelo aplicativo associado.|
|appId|Cadeia de caracteres|O identificador exclusivo do aplicativo associado (sua propriedade **appId**).|
|appRoleAssignmentRequired|Boolean|Especifica se um **appRoleAssignment** de um usuário ou grupo é necessário antes que o Azure AD emita um token de usuário ou de acesso ao aplicativo.                            **Observações**: requer a versão 1,5 ou posterior, não anulável.            |
|appRoles|appRole|As funções do aplicativo expostas pelo aplicativo associado. Para obter mais informações, consulte a definição da propriedade **appRoles** na entidade de aplicativo **observações**: requer a versão 1,5 ou posterior, não anulável.            |
|displayName|String|O nome de exibição da entidade de serviço.|
|errorUrl|String|            |
|homepage|String|A URL da home page do aplicativo associado.|
|keyCredentials|keyCredential|A coleção de credenciais principais associada à entidade de serviço.                            **Anotações**: não anulável.            |
|logoutUrl|String| Especifica a URL que será usada pela autorização do serviço da Microsoft para fazer logoff de um usuário usando protocolos de logoff [front-channel](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) ou SAML. |
|oauth2Permissions|oAuth2Permission|As permissões OAuth 2.0 expostas pelo aplicativo associado. Para obter mais informações, confira a definição da propriedade **oauth2Permissions** na entidade aplicativo.                            **Observações**: requer a versão 1,5 ou posterior, não anulável.            |
|passwordCredentials|passwordCredential|A coleção de credenciais de senha associada à entidade de serviço.                            **Anotações**: não anulável.            |
|preferredTokenSigningKeyThumbprint|String|Reservado apenas para uso interno. Não escreva ou dependa de alguma forma dessa propriedade. Pode ser removida em versões futuras.                            **Observações**: requer a versão 1,5 ou mais recente.            |
|publisherName|String|O nome de exibição do locatário no qual o aplicativo associado está especificado.|
|replyUrls|String|As URLs às quais os tokens de usuário são enviados para entrar com aplicativo associado ou os URIs de redirecionamento aos quais os códigos de autorização do OAuth 2.0 e tokens de acesso são enviados para o aplicativo associado.                            **Anotações**: não anulável.            |
|samlMetadataUrl|String|            |
|servicePrincipalNames|String|Os URIs que identificam o aplicativo associado. Para saber mais, confira [Objetos do aplicativo e objetos da entidade de serviço](https://msdn.microsoft.com/library/azure/dn132633.aspx).                            **Observações**: não nulos, o operador **any** é obrigatório para expressões de filtro em Propriedades de vários valores; para obter mais informações, consulte [supported queries, Filters, and paging Options](https://msdn.microsoft.com/library/azure/dn727074.aspx).            |
|marcações|String|                                        **Anotações**: não anulável.            |

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [servicePrincipalName](../resources/serviceprincipal.md) atualizado no corpo da resposta.
## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "update_serviceprincipal"
}-->
```http
PATCH https://graph.microsoft.com/beta/servicePrincipals/{id}
Content-type: application/json
Content-length: 391

{
  "accountEnabled": true,
  "addIns": [
    {
      "id": "id-value",
      "type": "type-value",
      "properties": [
        {
          "key": "key-value",
          "value": "value-value"
        }
      ]
    }
  ],
  "appDisplayName": "appDisplayName-value",
  "appId": "appId-value",
  "appOwnerOrganizationId": "appOwnerOrganizationId-value",
  "appRoleAssignmentRequired": true
}
```
##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 391

{
  "accountEnabled": true,
  "addIns": [
    {
      "id": "id-value",
      "type": "type-value",
      "properties": [
        {
          "key": "key-value",
          "value": "value-value"
        }
      ]
    }
  ],
  "appDisplayName": "appDisplayName-value",
  "appId": "appId-value",
  "appOwnerOrganizationId": "appOwnerOrganizationId-value",
  "appRoleAssignmentRequired": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update serviceprincipal",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
