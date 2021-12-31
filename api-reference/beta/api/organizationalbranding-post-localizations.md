---
title: Criar organizationalBrandingLocalization
description: Crie um novo objeto organizationalBrandingLocalization.
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: bcc093ed5487a2e2aeabcb230452b80a072411bd
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/30/2021
ms.locfileid: "61647032"
---
# <a name="create-organizationalbrandinglocalization"></a>Criar organizationalBrandingLocalization
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie um novo [objeto organizationalBrandingLocalization.](../resources/organizationalBrandingLocalization.md) Isso cria uma identidade visual localizada e, ao mesmo tempo, a identidade visual padrão se ela não existir.

A identidade visual padrão é criada apenas uma vez. Ele é carregado quando uma identidade visual localizada não é configurada para o idioma do navegador do usuário. Para recuperar a identidade visual padrão, consulte [Obter identidade visual](organizationalbranding-get.md).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Organization.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP
Essa solicitação cria uma nova identidade visual de localização e uma identidade visual padrão se ainda não existir. 
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /organization/{organizationId}/branding/localizations
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

A tabela a seguir mostra as propriedades que são necessárias ao criar o [objeto organizationalBrandingLocalization.](../resources/organizationalbrandinglocalization.md)

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| id | String | Um identificador que representa a localidade especificada usando nomes de cultura. Os nomes de cultura seguem o padrão RFC 1766 no formato "languagecode2-country/regioncode2", onde "languagecode2" é um código de duas letras minúsculo derivado da ISO 639-1 e "country/regioncode2" é um código de duas letras maiúscula derivado da ISO 3166. Por exemplo, inglês dos EUA é `en-US` . Não é possível criar a identidade visual padrão definindo o valor da **id** para os tipos de cadeia de caracteres `0` ou `default` .  <br/><br/>**OBSERVAÇÃO:** No momento, não há suporte para várias marcas para uma única localidade. |

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

O exemplo a seguir cria uma localização de identidade visual para localização em francês ( `fr-FR` ) . Quaisquer propriedades não especificadas do tipo String herdam do valor no objeto de identidade visual padrão. Por exemplo, se o signInPageText no objeto de identidade visual padrão for `null` , o signInPageText para a identidade visual criada nesta solicitação também `fr-FR` será `null` . Para substituir um `null` valor sem qualquer texto, use uma cadeia de caracteres que contenha apenas espaço em branco.

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_organizationalbrandinglocalization"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/beta/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations
Content-Type: application/json

{
    "backgroundColor":"#00000F",
    "id": "fr-FR",
    "signInPageText": " "
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-organizationalbrandinglocalization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-organizationalbrandinglocalization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-organizationalbrandinglocalization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-organizationalbrandinglocalization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.organizationalBrandingLocalization"
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#organization('d69179bf-f4a4-41a9-a9de-249c0f2efb1d')/branding/localizations/$entity",
    "@odata.id": "https://graph.microsoft.com/v2/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/directoryObjects/$/Microsoft.DirectoryServices.Organization('d69179bf-f4a4-41a9-a9de-249c0f2efb1d')//localizations/fr-FR",
    "id": "fr-FR",
    "backgroundColor": "",
    "backgroundImageRelativeUrl": null,
    "bannerLogoRelativeUrl": null,
    "cdnList": [],
    "signInPageText": " ",
    "squareLogoRelativeUrl": null,
    "usernameHintText": ""
}
```
