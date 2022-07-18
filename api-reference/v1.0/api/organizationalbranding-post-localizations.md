---
title: Criar organizationalBrandingLocalization
description: Crie um novo objeto organizationalBrandingLocalization.
author: AlexanderMars
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 8a2bba2591aefa4bc5dfd5821f8358af66e82dc3
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66439246"
---
# <a name="create-organizationalbrandinglocalization"></a>Criar organizationalBrandingLocalization
Namespace: microsoft.graph

Crie um novo [objeto organizationalBrandingLocalization](../resources/organizationalBrandingLocalization.md) . Isso cria uma identidade visual localizada e, ao mesmo tempo, a identidade visual padrão, se ela não existir.

A identidade visual padrão é criada apenas uma vez. Ele é carregado quando uma identidade visual localizada não está configurada para o idioma do navegador do usuário. Para recuperar a identidade visual padrão, consulte [Obter identidade visual](organizationalbranding-get.md).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Organization.ReadWrite.All |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP
Essa solicitação cria uma nova identidade visual de localização e uma identidade visual padrão, caso ainda não exista uma. 
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

A tabela a seguir mostra as propriedades que são necessárias ao criar o objeto [organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) .

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| id | Cadeia de caracteres | Um identificador que representa a localidade especificada usando nomes de cultura. Os nomes de cultura seguem o padrão RFC 1766 no formato "languagecode2-country/regioncode2", em que "languagecode2" é um código de duas letras minúsculas derivado da ISO 639-1 e "country/regioncode2" é um código de duas letras maiúsculas derivado da ISO 3166. Por exemplo, inglês americano é `en-US`. Você não pode criar a identidade visual padrão definindo o valor da **ID** para os tipos de cadeia de caracteres `0` ou `default`.  <br/><br/>**NOTA:** No momento, não há suporte para várias marcas para uma única localidade. |

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `201 Created` de resposta e um [objeto organizationalBrandingLocalization](../resources/organizationalbrandinglocalization.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

O exemplo a seguir cria uma localização de identidade visual para localização em francês (`fr-FR`). Todas as propriedades não especificadas do tipo String herdam do valor no objeto de identidade visual padrão. Por exemplo, se o signInPageText no objeto de identidade visual `null`padrão for , o signInPageText `fr-FR` para a identidade visual criada nesta solicitação também será `null`. Para substituir um valor `null` sem nenhum texto, use uma cadeia de caracteres que contenha apenas espaço em branco.

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_organizationalbrandinglocalization"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/organization/d69179bf-f4a4-41a9-a9de-249c0f2efb1d/branding/localizations
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

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-organizationalbrandinglocalization-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/create-organizationalbrandinglocalization-powershell-snippets.md)]
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#organization('d69179bf-f4a4-41a9-a9de-249c0f2efb1d')/branding/localizations/$entity",
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
