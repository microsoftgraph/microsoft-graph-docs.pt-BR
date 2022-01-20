---
title: Atualizar countryNamedlocation
description: Atualize as propriedades de um objeto countryNamedLocation.
ms.localizationpriority: medium
author: videor
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 5bdb25a2a429dfbf699e469307ab4282eee72d86
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62126380"
---
# <a name="update-countrynamedlocation"></a>Atualizar countryNamedLocation

Namespace: microsoft.graph

Atualize as propriedades de um [objeto countryNamedLocation.](../resources/countryNamedLocation.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Policy.Read.All e Policy.ReadWrite.ConditionalAccess |
| Delegado (conta pessoal da Microsoft) | Sem suporte. |
| Aplicativo                            | Policy.Read.All e Policy.ReadWrite.ConditionalAccess |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/conditionalAccess/namedLocations/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Descrição|
|:-----------|:-----------|
| Autorização | {token} de portador. Obrigatório. |
| Content-type  | application/json. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.

Você deve especificar o **@odata.type** como `#microsoft.graph.countryNamedLocation` .

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|countriesAndRegions|Coleção de cadeias de caracteres|Lista de países e/ou regiões no formato de duas letras especificado pela ISO 3166-2.|
|displayName|Cadeia de caracteres|Nome acessível para humanos do local.|
|includeUnknownCountriesAndRegions|Booliano|O valor é `true` se os endereços IP que não mapeiam para um país ou região devem ser incluídos no local nomeado.|

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_countrynamedlocation"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/identity/conditionalAccess/namedLocations/1c4427fd-0885-4a3d-8b23-09a899ffa959
Content-type: application/json

{
    "@odata.type": "#microsoft.graph.countryNamedLocation",
    "displayName": "Updated named location without unknown countries and regions",
    "countriesAndRegions": [
        "CA",
        "IN"
    ],
    "includeUnknownCountriesAndRegions": false
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-countrynamedlocation-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-countrynamedlocation-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-countrynamedlocation-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-countrynamedlocation-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-countrynamedlocation-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-countrynamedlocation-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update countrynamedlocation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

