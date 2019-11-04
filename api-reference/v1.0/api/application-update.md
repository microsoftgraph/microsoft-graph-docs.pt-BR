---
title: Atualizar aplicativo
description: Atualiza as propriedades de um objeto Application.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 387b5be3bd8de1158eb47a6690df9a96a52691e8
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939667"
---
# <a name="update-application"></a>Atualizar aplicativo

Atualiza as propriedades de um objeto [Application](../resources/application.md) .
## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).


|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |  Directory.AccessAsUser.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | Application.ReadWrite.OwnedBy, Application.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PATCH /applications/{id}
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Descrição|
|:-----------|:----------|
| Autorização | {token} de portador. Obrigatório.  |
| Content-type | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade | Tipo | Descrição |
|:---------------|:--------|:----------|
| api | [apiApplication](../resources/apiapplication.md) | Especifica configurações para um aplicativo que implementa uma API Web. |
| appRoles | Coleção [appRole](../resources/approle.md) | A coleção de funções de aplicativo que um aplicativo pode declarar. Essas funções podem ser atribuídas a usuários, grupos ou entidades de serviço. Não anulável. |
| displayName | Cadeia de caracteres | O nome de exibição do aplicativo. |
| groupMembershipClaims | Cadeia de caracteres | Configura a declaração de **grupos** emitida em um usuário ou token de acesso do OAuth 2,0 que o aplicativo espera. Para definir esse atributo, use um dos seguintes valores válidos de cadeia de caracteres:<ul><li>`None`</li><li>`SecurityGroup`: Para grupos de segurança e funções do Azure Active Directory (Azure AD)</li><li>`All`: Isso obterá todos os grupos de segurança, grupos de distribuição e funções de diretório do Azure AD dos quais o usuário conectado é membro</li></ul> |
| identifierUris | Coleção String | Os URIs que identificam o aplicativo em seu locatário do Azure AD ou em um domínio personalizado verificado se o aplicativo for multilocatário. Para obter mais informações, consulte [Application Objects and Service principal Objects](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals). O operador *any* é obrigatório para expressões de filtro em propriedades de vários valores. Não anulável. |
| informações  | [informationalUrl](../resources/informationalurl.md) | Informações básicas de perfil do aplicativo, como marketing do aplicativo, suporte, termos de serviço e URLs da declaração de privacidade. Os termos de serviço e declaração de privacidade são reproduzidos para os usuários por meio da experiência de consentimento do usuário. Para obter mais informações, consulte [Adicionar termos de serviço e declaração de privacidade para aplicativos registrados do Azure ad](https://docs.microsoft.com/azure/active-directory/develop/howto-add-terms-of-service-privacy-statement). |
| isFallbackPublicClient | Booliano | Especifica o tipo de aplicativo de fallback como cliente público, como um aplicativo instalado em execução em um dispositivo móvel. O valor padrão é `false`, que significa que o tipo de aplicativo de fallback é um cliente confidencial, como o aplicativo Web. Há determinados cenários em que o Azure AD não pode determinar o tipo de aplicativo cliente (por exemplo, [ROPC](https://tools.ietf.org/html/rfc6749#section-4.3) Flow onde ele é configurado sem especificar um URI de redirecionamento). Nesses casos, o Azure AD interpretará o tipo de aplicativo com base no valor dessa propriedade.|
| keyCredentials | [keyCredential](../resources/keycredential.md) collection | O conjunto de credenciais chave associadas ao aplicativo. Não anulável. |
| logo | Stream | O principal logotipo do aplicativo. Não anulável. |
| optionalClaims | optionalClaims | Os desenvolvedores de aplicativos podem configurar declarações opcionais em seus aplicativos do Azure AD para especificar quais declarações eles desejam em tokens enviados para seus aplicativos pelo serviço de token de segurança da Microsoft. Consulte [declarações opcionais](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims) para obter mais informações. |
| parentalControlSettings | [parentalControlSettings](../resources/parentalcontrolsettings.md) |Especifica as configurações de controle parental de um aplicativo. |
| passwordCredentials | Coleção [passwordCredential](../resources/passwordcredential.md)|A coleção de credenciais de senha associada ao aplicativo. Não anulável.|
| publicClient | [publicClientApplication](../resources/publicclientapplication.md) | Especifica configurações para clientes instalados, como dispositivos móveis ou da área de trabalho. |
| requiredResourceAccess |[requiredResourceAccess](../resources/requiredresourceaccess.md) collection|Especifica os recursos para os quais esse aplicativo requer acesso e o conjunto de escopos de permissão e funções de aplicativo do OAuth necessários em cada um desses recursos. Essa pré-configuração de acesso necessário aos recursos impulsiona a experiência de consentimento. Não anulável.|
| signInAudience | String | Especifica a quais contas da Microsoft são compatíveis com o aplicativo atual. Os valores compatíveis são:<ul><li>`AzureADMyOrg`: Usuários com uma conta corporativa ou de estudante da Microsoft no locatário do Azure AD da minha organização (ou seja, um único locatário)</li><li>`AzureADMultipleOrgs`: Usuários com uma conta corporativa ou de estudante da Microsoft no locatário do Azure AD de qualquer organização (ou seja, multilocatário)</li> <li>`AzureADandPersonalMicrosoftAccount`: Usuários com uma conta pessoal da Microsoft ou uma conta corporativa ou de estudante no locatário do Azure AD de qualquer organização</li></ul> | `AzureADandPersonalMicrosoftAccount` |
| tags |Coleção String| Sequências personalizadas que podem ser usadas para categorizar e identificar o aplicativo. Não anulável.|
| tokenEncryptionKeyId |Cadeia de caracteres|Especifica o keyId de uma chave pública da coleção keycredentials. Quando configurado, o Azure AD criptografa todos os tokens emitidos usando a chave para a qual essa propriedade aponta. O código do aplicativo que recebe o token criptografado deve usar a chave privada correspondente para descriptografar o token antes que possa ser usado para o usuário conectado.|
| web |[webApplication](../resources/webapplication.md)| Especifica configurações para um aplicativo Web. |

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará `204 No Content` um código de resposta e não retornará nada no corpo da resposta.
## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.

<!-- {
  "blockType": "request",
  "name": "update_application"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/applications/{id}
Content-type: application/json
Content-length: 72

{
  "displayName": "New display name"
}
```

##### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
