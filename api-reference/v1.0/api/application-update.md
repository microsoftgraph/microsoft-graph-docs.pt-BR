---
title: Atualizar aplicativo
description: Atualize as propriedades de um objeto application.
author: sureshja
ms.localizationpriority: medium
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 2f3aedf415e0086e506729f13b7ca1ce94257dd2
ms.sourcegitcommit: 11be55b40804b07f4c422f09f601afa97c7d31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2021
ms.locfileid: "60256162"
---
# <a name="update-application"></a>Atualizar aplicativo

Namespace: microsoft.graph

Atualize as propriedades de um [objeto application.](../resources/application.md)

> [!IMPORTANT]
> Não há suporte para o uso do PATCH para definir [**passwordCredential**](../resources/passwordcredential.md). Use os [métodos addPassword](./application-addpassword.md) e [removePassword](./application-removepassword.md) para atualizar a senha de um aplicativo.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).


|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante) |  Application.ReadWrite.All, Directory.AccessAsUser.All    |
|Delegada (conta pessoal da Microsoft) | Application.ReadWrite.All |
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
| Content-Type | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade                | Tipo                                                                        | Descrição                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
|:------------------------|:----------------------------------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| api                     | [apiApplication](../resources/apiapplication.md)                            | Especifica configurações para um aplicativo que implementa uma API Web.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| appRoles                | Coleção [appRole](../resources/approle.md)                               | A coleção de funções de aplicativo que um aplicativo pode declarar. Essas funções podem ser atribuídas a usuários, grupos ou entidades de serviço. Não anulável.                                                                                                                                                                                                                                                                                                                                                                                                                |
| displayName             | String                                                                      | O nome de exibição do aplicativo.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| groupMembershipClaims   | Cadeia de caracteres                                                                      | Configura a declaração **de grupos** emitida em um usuário ou token de acesso OAuth 2.0 que o aplicativo espera. Para definir esse atributo, use um dos seguintes valores válidos de cadeia de caracteres:<ul><li>`None`</li><li>`SecurityGroup`: Para grupos de segurança e Azure Active Directory funções (Azure AD)</li><li>`All`: isso obterá todos os grupos de segurança e de distribuição e funções de diretório do Azure AD dos quais o usuário conectado é membro.</li></ul>                                                                                                                       |
| identifierUris          | Coleção de cadeias de caracteres                                                           | Os URIs que identificam o aplicativo em seu locatário do Azure AD ou em um domínio personalizado verificado, se o aplicativo é multilocatário. Para saber mais, confira [Objetos de aplicativo e Objetos de entidade de serviço](/azure/active-directory/develop/app-objects-and-service-principals). O operador *any* é obrigatório para expressões de filtro em propriedades de vários valores. Não anulável.                                                                                                                                                                           |
| informações                     | [informationalUrl](../resources/informationalurl.md)                        | Informações básicas de perfil do aplicativo, como URLs de marketing, suporte, termos de serviço e declaração de privacidade do aplicativo. Os termos de serviço e a política de privacidade são revelados aos usuários por meio da experiência de consentimento do usuário. Para obter mais informações, [consulte Add Terms of service and privacy statement for registered Azure AD apps](/azure/active-directory/develop/howto-add-terms-of-service-privacy-statement).                                                                                                                                                 |
| isFallbackPublicClient  | Booliano                                                                     | Especifica o tipo de aplicativo de fallback como cliente público; por exemplo, um aplicativo instalado em um dispositivo móvel. O valor padrão é , o que significa que o tipo de `false` aplicativo de fallback é cliente confidencial, como aplicativo Web. Há certos cenários em que o Azure AD não pode determinar o tipo de aplicativo cliente (por exemplo, o fluxo [ropc](https://tools.ietf.org/html/rfc6749#section-4.3) em que ele é configurado sem especificar um URI de redirecionamento). Nesses casos, o Azure AD interpretará o tipo de aplicativo com base no valor dessa propriedade. |
| keyCredentials          | [keyCredential](../resources/keycredential.md) collection                   | A coleção das principais credenciais associadas ao aplicativo. Não anulável.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| logo                    | Stream                                                                      | O logotipo principal do aplicativo. Não anulável.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| optionalClaims          | optionalClaims                                                              | Desenvolvedores de aplicativos podem configurar declarações opcionais em aplicativos do Azure AD para especificar quais declarações desejam em tokens enviados ao aplicativo pelo serviço de token de segurança da Microsoft. Consulte [declarações opcionais](/azure/active-directory/develop/active-directory-optional-claims) para obter mais informações.                                                                                                                                                                                                                                                               |
| parentalControlSettings | [parentalControlSettings](../resources/parentalcontrolsettings.md)          | Especifica as configurações de controle parental de um aplicativo.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| publicClient            | [publicClientApplication](../resources/publicclientapplication.md)          | Especifica configurações para clientes instalados, como dispositivos móveis ou da área de trabalho.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| requiredResourceAccess  | [requiredResourceAccess](../resources/requiredresourceaccess.md) collection | Especifique os recursos que o aplicativo precisa acessar. Essa propriedade também especifica o conjunto de permissões delegadas e funções de aplicativo que ela precisa para cada um desses recursos. Essa configuração de acesso aos recursos necessários impulsiona a experiência de consentimento. Não é possível configurar mais de 50 serviços de recursos (APIs). A partir de meados de outubro de 2021, o número total de permissões necessárias não deve exceder 400. Não anulável.                                                                                                                 |
| signInAudience          | String                                                                      | Especifica a quais contas da Microsoft são compatíveis com o aplicativo atual. Os valores compatíveis são:<ul><li>`AzureADMyOrg`: usuários com uma conta corporativa ou de estudante da Microsoft no locatário do Azure AD da organização (ou seja, locatário único)</li><li>`AzureADMultipleOrgs`: usuários com uma conta corporativa ou de estudante da Microsoft no locatário do Azure AD da organização (ou seja, multilocatário)</li> <li>`AzureADandPersonalMicrosoftAccount`: usuários com uma conta Microsoft pessoal ou uma conta corporativa ou de estudante no locatário do Azure AD de qualquer organização</li></ul>                           |
| tags                    | Coleção String                                                           | Cadeias de caracteres personalizadas que podem ser usadas para categorizar e identificar o aplicativo. Não anulada.                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| tokenEncryptionKeyId    | Cadeia de caracteres                                                                      | Especifica a keyId de uma chave pública da coleção keyCredentials. Quando configurado, o Azure AD criptografa todos os tokens emitidos usando a chave para a qual essa propriedade aponta. O código de aplicativo que recebe o token criptografado deve usar a chave privada correspondente para descriptografar o token a fim de que ele possa ser usado para o usuário conectado.                                                                                                                                                                                                                               |
| web                     | [webApplication](../resources/webapplication.md)                            | Especifica configurações para um aplicativo Web.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `204 No Content` de resposta e não retornará nada no corpo da resposta.
## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.


# <a name="http"></a>[HTTP](#tab/http)
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>Resposta

<!-- {
  "blockType": "response"
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
