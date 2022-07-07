---
title: Atualizar aplicativo
description: Atualize as propriedades de um objeto de aplicativo.
author: sureshja
ms.localizationpriority: medium
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 5eca1c3b8455bc2b9ba9694a7beb4b2f1132e84f
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66670327"
---
# <a name="update-application"></a>Atualizar aplicativo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades de um [objeto de](../resources/application.md) aplicativo.

> [!IMPORTANT]
> Não há suporte para o uso do PATCH para definir [**passwordCredential**](../resources/passwordcredential.md). Use os [métodos addPassword](./application-addpassword.md) [e removePassword](./application-removepassword.md) para atualizar a senha ou o segredo de um aplicativo.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).


|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) |  Application.ReadWrite.All, Directory.ReadWrite.All |
|Delegado (conta pessoal da Microsoft) | Application.ReadWrite.All    |
|Aplicativo | Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
Substitua `{id}` pela **ID** do objeto de aplicativo, também conhecida como a **ID de Objeto** no portal do Azure.
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
| groupMembershipClaims   | Cadeia de caracteres                                                                      | Configura a declaração **de grupos** emitida em um usuário ou token de acesso OAuth 2.0 que o aplicativo espera. Para definir esse atributo, use um dos seguintes valores válidos de cadeia de caracteres:<ul><li>`None`</li><li>`SecurityGroup`: para grupos de segurança e funções do Azure Active Directory (Azure AD)</li><li>`All`: isso obterá todos os grupos de segurança e de distribuição e funções de diretório do Azure AD dos quais o usuário conectado é membro.</li></ul>                                                                                                                       |
| identifierUris          | Coleção de cadeias de caracteres                                                           | Os URIs que identificam o aplicativo em seu locatário do Azure AD ou em um domínio personalizado verificado, se o aplicativo é multilocatário. Para saber mais, confira [Objetos de aplicativo e Objetos de entidade de serviço](/azure/active-directory/develop/app-objects-and-service-principals). O operador *any* é obrigatório para expressões de filtro em propriedades de vários valores. Não anulável.                                                                                                                                                                           |
| informações                     | [informationalUrl](../resources/informationalurl.md)                        | Informações básicas de perfil do aplicativo, como marketing, suporte, termos de serviço e URLs de política de privacidade do aplicativo. Os termos de serviço e a política de privacidade são revelados aos usuários por meio da experiência de consentimento do usuário. Para obter mais informações, consulte [Adicionar Termos de serviço e política de privacidade para aplicativos Azure AD registrados](/azure/active-directory/develop/howto-add-terms-of-service-privacy-statement).                                                                                                                                                 |
| isFallbackPublicClient  | Booliano                                                                     | Especifica o tipo de aplicativo de fallback como cliente público; por exemplo, um aplicativo instalado em um dispositivo móvel. O valor padrão é `false`, o que significa que o tipo de aplicativo de fallback é cliente confidencial, como o aplicativo Web. Há determinados cenários em que Azure AD pode determinar o tipo de aplicativo cliente (por exemplo, o fluxo [ROPC](https://tools.ietf.org/html/rfc6749#section-4.3) em que ele está configurado sem especificar um URI de redirecionamento). Nesses casos, Azure AD interpretará o tipo de aplicativo com base no valor dessa propriedade. |
| keyCredentials          | [keyCredential](../resources/keycredential.md) collection                   | A coleção das principais credenciais associadas ao aplicativo. Não anulável.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| logo                    | Stream                                                                      | O logotipo principal do aplicativo. Não anulável.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| onPremisesPublishing    | [onPremisesPublishing](../resources/onpremisespublishing.md)                | Representa o conjunto de propriedades para configurar [Azure AD Proxy de Aplicativo](/azure/active-directory/app-proxy/what-is-application-proxy) para um aplicativo local. Essa propriedade só pode ser definida após a criação do aplicativo e não pode ser atualizada na mesma solicitação que outras propriedades do aplicativo.                                                                                                                                                                                                                                                                                                                                                       |
| optionalClaims          | optionalClaims                                                              | Desenvolvedores de aplicativos podem configurar declarações opcionais em aplicativos do Azure AD para especificar quais declarações desejam em tokens enviados ao aplicativo pelo serviço de token de segurança da Microsoft. Consulte [declarações opcionais](/azure/active-directory/develop/active-directory-optional-claims) para obter mais informações.                                                                                                                                                                                                                                                               |
| parentalControlSettings | [parentalControlSettings](../resources/parentalcontrolsettings.md)          | Especifica as configurações de controle parental de um aplicativo.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| publicClient            | [publicClientApplication](../resources/publicclientapplication.md)          | Especifica configurações para clientes instalados, como dispositivos móveis ou da área de trabalho.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| requiredResourceAccess  | [requiredResourceAccess](../resources/requiredresourceaccess.md) collection | Especifique os recursos que o aplicativo precisa acessar. Essa propriedade também especifica o conjunto de permissões delegadas e funções de aplicativo necessárias para cada um desses recursos. Essa configuração de acesso aos recursos necessários impulsiona a experiência de consentimento. Não é possível configurar mais de 50 APIs (serviços de recursos). A partir de meados de outubro de 2021, o número total de permissões necessárias não deve exceder 400. Não anulável.                                                                                                                 |
| samlMetadataUrl | Cadeia de caracteres | A URL em que o serviço expõe os metadados SAML para federação. Essa propriedade é válida apenas para aplicativos de locatário único. |
| signInAudience          | String                                                                      | Especifica a quais contas da Microsoft são compatíveis com o aplicativo atual. Os valores compatíveis são:<ul><li>`AzureADMyOrg`: usuários com uma conta corporativa ou de estudante da Microsoft no locatário do Azure AD da organização (ou seja, locatário único)</li><li>`AzureADMultipleOrgs`: usuários com uma conta corporativa ou de estudante da Microsoft no locatário do Azure AD da organização (ou seja, multilocatário)</li> <li>`AzureADandPersonalMicrosoftAccount`: usuários com uma conta Microsoft pessoal ou uma conta corporativa ou de estudante no locatário do Azure AD de qualquer organização</li></ul>                           |
| spa                     | [spaApplication](../resources/spaapplication.md)                            | Especifica as configurações de um aplicativo de página simples, incluindo URLs de saída e de redirecionamento de URIs para os códigos de autorização e tokens de acesso. |
| categorias                    | Coleção String                                                           | Cadeias de caracteres personalizadas que podem ser usadas para categorizar e identificar o aplicativo. Não anulada.                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| tokenEncryptionKeyId    | Cadeia de caracteres                                                                      | Especifica a keyId de uma chave pública da coleção keyCredentials. Quando configurado, o Azure AD criptografa todos os tokens emitidos usando a chave para a qual essa propriedade aponta. O código de aplicativo que recebe o token criptografado deve usar a chave privada correspondente para descriptografar o token a fim de que ele possa ser usado para o usuário conectado.                                                                                                                                                                                                                               |
| Nome único | Cadeia de caracteres | O identificador exclusivo que pode ser atribuído a um aplicativo como um identificador alternativo. Imutável. Somente leitura.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| web                     | [webApplication](../resources/webapplication.md)                            | Especifica configurações para um aplicativo Web.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| spa                     | [spaApplication](../resources/spaapplication.md)                            | Especifica as configurações de um aplicativo de página simples, incluindo URLs de saída e de redirecionamento de URIs para os códigos de autorização e tokens de acesso. |
| windows                     | [windowsApplication](../resources/windowsapplication.md)                            | Especifica as configurações dos aplicativos que executam o Microsoft Windows e publicados no Microsoft Store ou no armazenamento de jogos do Xbox. Inclui SID do pacote e URIs de redirecionamento para códigos de autorização e tokens de acesso. |

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `204 No Content` código de resposta e não retornará nada no corpo da resposta.
## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_application"
}-->
```http
PATCH https://graph.microsoft.com/beta/applications/{id}
Content-type: application/json

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

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-application-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-application-powershell-snippets.md)]
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
