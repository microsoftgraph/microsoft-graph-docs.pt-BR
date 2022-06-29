---
title: Atualizar organizationalBrandingLocalization
description: Atualize as propriedades de um objeto organizationalBrandingLocalization.
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 8fa2a1eb9f22c1055bb99666f4845a3a8505ffe0
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66443302"
---
# <a name="update-organizationalbrandinglocalization"></a>Atualizar organizationalBrandingLocalization
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades de um [objeto organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) para uma localização específica.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegada (conta corporativa ou de estudante)     | Organization.ReadWrite.All |
| Delegada (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

Somente os tipos de dados do Stream, incluindo **backgroundLogo** e **backgroundImage**, são atualizados usando o método PUT. Para atualizar tipos de dados de cadeia de caracteres, incluindo **signInPageText** e **usernameHintText**, use o método PATCH. Não é possível atualizar tipos de fluxo com outros tipos de dados na mesma solicitação.

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}/branding/localizations/{organizationalBrandingLocalizationId}
PUT /organization/{organizationId}/branding/localizations/{organizationalBrandingLocalizationId}/{backgroundImage | bannerLogo | squareLogo}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| Backgroundcolor | Cadeia de caracteres | Cor que aparece no lugar da imagem de plano de fundo em conexões de baixa largura de banda. Recomendamos que você use a cor principal do logotipo da faixa ou da cor da sua organização. Especifique isso no formato hexadecimal, por exemplo, branco é `#FFFFFF`. |
| Backgroundimage | Stream | Imagem que aparece como a tela de fundo da página de entrada. Os tipos permitidos são PNG ou JPEG não menores que 300 KB e não maiores que 1920 × 1080 pixels. Uma imagem menor reduzirá os requisitos de largura de banda e fará com que o carregamento da página seja mais rápido. |
| bannerLogo | Stream | Uma versão em faixa do logotipo da sua empresa que aparece na página de entrada. Os tipos permitidos são PNG ou JPEG não maiores que 36 × 245 pixels. É recomendável usar uma imagem transparente sem preenchimento ao redor do logotipo. |
| customAccountResetCredentialsUrl | String | Uma URL personalizada para redefinir as credenciais da conta. Essa URL deve estar no formato ASCII ou caracteres não ASCII devem ser codificados em URL e não exceder 128 caracteres. |
| customCannotAccessYourAccountText | Cadeia de caracteres | Uma cadeia de caracteres para substituir o padrão "Não é possível acessar sua conta?" texto de hiperlink de redefinição de senha de autoatendimento (SSPR) na página de entrada. Esse texto deve estar no formato Unicode e não exceder 256 caracteres. |
| customForgotMyPasswordText | Cadeia de caracteres | Uma cadeia de caracteres para substituir o texto padrão do hiperlink "Esqueci minha senha" no formulário de entrada. Esse texto deve estar no formato Unicode e não exceder 256 caracteres. |
| customPrivacyAndCookiesText | String | Uma cadeia de caracteres para substituir o texto padrão do hiperlink "Privacidade e Cookies" no rodapé. Esse texto deve estar no formato Unicode e não exceder 256 caracteres. |
| customPrivacyAndCookiesUrl | Cadeia de caracteres | Uma URL personalizada para substituir a URL padrão do hiperlink "Privacidade e Cookies" no rodapé. Essa URL deve estar no formato ASCII ou caracteres não ASCII devem ser codificados em URL e não exceder 128 caracteres. |
| customTermsOfUseText | Cadeia de caracteres | Uma cadeia de caracteres para substituir o texto padrão do hiperlink "Termos de Uso" no rodapé. Esse texto deve estar no formato Unicode e não exceder 256 caracteres. |
| customTermsOfUseUrl | Cadeia de caracteres | Uma URL personalizada para substituir a URL padrão do hiperlink "Termos de Uso" no rodapé. Essa URL deve estar no formato ASCII ou caracteres não ASCII devem ser codificados em URL e não exceder 128 caracteres. |
| Favicon | Stream | Um ícone personalizado (favicon) para substituir um favicon de produto padrão da Microsoft em um Azure AD locatário. |
| headerBackgroundColor | Cadeia de caracteres | A cor RGB a ser aplicada para personalizar a cor do cabeçalho. |
| loginPageTextVisibilitySettings | [loginPageTextVisibilitySettings](../resources/loginPageTextVisibilitySettings.md) | Representa os vários textos que podem ser ocultos na página de logon de um locatário. Todas as propriedades podem ser atualizadas. |
| signInPageText | Cadeia de caracteres | Texto que aparece na parte inferior da caixa de entrada. Use isso para comunicar informações adicionais, como o número de telefone para o suporte de assistência técnica ou uma declaração legal. Esse texto deve estar no formato Unicode e não exceder 1024 caracteres. |
| squareLogo | Stream | Uma versão quadrada do logotipo da sua empresa que aparece Windows 10 OOBE (experiências integradas) e quando o Windows Autopilot está habilitado para implantação. Os tipos permitidos são PNG ou JPEG não maiores que 240 x 240 pixels e não têm mais de 10 KB de tamanho. É recomendável usar uma imagem transparente sem preenchimento ao redor do logotipo.|
| usernameHintText | Cadeia de caracteres | Uma cadeia de caracteres que mostra como a dica na caixa de texto de nome de usuário na tela de entrada. Esse texto deve ser um Unicode, sem links ou código, e não pode exceder 64 caracteres. |

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="example-1-setting-bannerlogo-for-the-fr-fr-localization-using-put"></a>Exemplo 1: **Definindo bannerLogo** para a localização fr-FR usando PUT

A solicitação a seguir atualiza o logotipo da faixa para a localização fr-FR.

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandinglocalization"
}-->

```msgraph-interactive
PUT https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr-FR/bannerLogo
Content-Type: image/jpeg

<Image>
```

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="example-2-update-the-backgroundcolor-and-signinpagetext-for-the-fr-fr-localization-using-patch"></a>Exemplo 2: atualizar backgroundColor e signInPageText para a localização fr-FR usando PATCH

A solicitação a seguir atualiza o logotipo da faixa para a `fr-FR` localização.

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandinglocalization6"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr-FR
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "signInPageText": "Welcome to Contoso France"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandinglocalization6-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandinglocalization6-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandinglocalization6-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandinglocalization6-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-organizationalbrandinglocalization6-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-organizationalbrandinglocalization6-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```



### <a name="example-3-override-a-default-branding-value-with-a-blank-string"></a>Exemplo 3: Substituir um valor de identidade visual padrão por uma cadeia de caracteres em branco

#### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_organizationalbrandinglocalization7"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations/fr-FR
Content-Type: application/json

{
    "signInPageText": "Welcome to Contoso France.",
    "usernameHintText":" "
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-organizationalbrandinglocalization7-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-organizationalbrandinglocalization7-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-organizationalbrandinglocalization7-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-organizationalbrandinglocalization7-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-organizationalbrandinglocalization7-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-organizationalbrandinglocalization7-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>Resposta

Após a solicitação, **o usernameHintText** `fr-FR` para a localização estará vazio em vez de herdar o valor do objeto de identidade visual padrão.

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```
