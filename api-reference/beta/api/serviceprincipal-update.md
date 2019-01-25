---
title: Atualizar serviceprincipal
description: Atualize as propriedades do objeto serviceprincipal.
localization_priority: Normal
ms.openlocfilehash: a562bca03881923cfc21d32eadee2a7f7053fa9b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511657"
---
# <a name="update-serviceprincipal"></a>Atualizar serviceprincipal

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades do objeto serviceprincipal.
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
|accountEnabled|Booliano|                **true** se a conta de serviço principal estiver ativada; Caso contrário, **false**.            |
|AppDisplayName|String|O nome de exibição exposto pelo aplicativo associado.|
|appId|String|O identificador exclusivo para o aplicativo associado (sua propriedade **appId** ).|
|appRoleAssignmentRequired|Booliano|Especifica se um **appRoleAssignment** a um usuário ou grupo é necessária antes que o Azure AD emitirá um usuário ou um token de acesso ao aplicativo.                            **Observações**: requer a versão 1.5 ou mais recente, não são nulas.            |
|appRoles|appRole|As funções do aplicativo expostas pelo aplicativo associado. Para obter mais informações, consulte a definição da propriedade **appRoles** sobre a entidade de aplicativo **Notes**: requer a versão 1.5 ou mais recente, não são nulas.            |
|displayName|String|O nome de exibição para a entidade de serviço.|
|errorUrl|String|            |
|HomePage|String|A URL para a home page do aplicativo associado.|
|keyCredentials|keyCredential|A coleção de credenciais de chave associado ao serviço principal.                            **Anotações**: não anulável.            |
|logoutUrl|String| Especifica a URL que será usada pelo serviço de autorização da Microsoft para logout um usuário usando o [canal de frente](https://openid.net/specs/openid-connect-frontchannel-1_0.html), [back-channel](https://openid.net/specs/openid-connect-backchannel-1_0.html) ou protocolos de logout SAML. |
|oauth2Permissions|oAuth2Permission|As permissões de OAuth 2.0 expostas pelo aplicativo associado. Para obter mais informações, consulte a definição da propriedade **oauth2Permissions** sobre a entidade de aplicativo.                            **Observações**: requer a versão 1.5 ou mais recente, não são nulas.            |
|passwordCredentials|passwordCredential|A coleção de credenciais de senha associadas a entidade de serviço.                            **Anotações**: não anulável.            |
|preferredTokenSigningKeyThumbprint|String|Reservado para uso interno apenas. Não gravar ou caso contrário, contam com esta propriedade. Pode ser removido em futuras versões.                            **Observações**: requer a versão 1.5 ou mais recente.            |
|publisherName|Cadeia de caracteres|O nome de exibição do inquilino no qual o aplicativo associado for especificado.|
|replyUrls|String|As URLs que os tokens do usuário são enviados para entrada com o aplicativo associado ou o redirecionamento códigos de autorização de URIs que OAuth 2.0 e tokens de acesso são enviados para o aplicativo associado.                            **Anotações**: não anulável.            |
|samlMetadataUrl|String|            |
|servicePrincipalNames|String|Os URIs que identificam o aplicativo associado. Para mais informações, consulte [objetos de aplicativo e objetos de entidade de serviço](https://msdn.microsoft.com/library/azure/dn132633.aspx).                            **Observações**: não são nulas, o operador **any** é necessário para expressões de filtro propriedades de valores múltiplos; Para obter mais informações, consulte [suporte para consultas, filtros e opções de paginação](https://msdn.microsoft.com/library/azure/dn727074.aspx).            |
|marcações|String|                                        **Anotações**: não anulável.            |

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e o objeto atualizado [servicePrincipal](../resources/serviceprincipal.md) no corpo da resposta.
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
  "@odata.type": "microsoft.graph.serviceprincipal"
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
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
