---
title: 'informationProtectionLabel: extractLabel'
description: Recupere informationProtectionContentLabel usando metadados de um objeto rotulado.
ms.localizationpriority: medium
author: tommoser
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: a4629a32e3f4d91306e36b371744ffe93104f37d
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349186"
---
# <a name="informationprotectionlabel-extractlabel"></a>informationProtectionLabel: extractLabel

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usando os metadados existentes em uma informação já rotulada, resolva os metadados para um rótulo de sensibilidade específico. A [entrada contentInfo](../resources/contentinfo.md) é resolvida para [informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md).

>[!NOTE]
>O **[recurso informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md)** representa um rótulo de sensibilidade que foi aplicado a uma informação. [os objetos informationProtectionLabel](../resources/informationprotectionlabel.md) são os rótulos abstratos que fazem parte da política de rotulagem organizacional e podem ser aplicados às informações.

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
| :------------------------------------- | :------------------------------------------ |
| Delegado (conta corporativa ou de estudante)     | InformationProtectionPolicy. Read            |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                              |
| Aplicativo                            | InformationProtectionPolicy.Read.All        |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /informationprotection/policy/labels/extractLabel
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome          | Descrição                                                                                                                                                                       |
| :------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Autorização | {token} de portador. Obrigatório.                                                                                                                                                         |
| Content-type  | Tipo de conteúdo: application/json. Obrigatório.                                                                                                                                         |
| User-Agent    | Descreve o nome e a versão do aplicativo de chamada. Os detalhes aparecerão no Azure Information Protection Analytics. O formato sugerido é ApplicationName/Version. Opcional. |

## <a name="request-body"></a>Corpo da solicitação

Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.

| Parâmetro   | Tipo                                       | Descrição                                                                                                                         |
| :---------- | :----------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------- |
| contentInfo | [contentInfo](../resources/contentinfo.md) | Fornece detalhes sobre o formato de conteúdo, o estado do conteúdo e os [metadados](../resources/keyvaluepair.md) existentes como pares de chave/valor. |

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e um novo [objeto informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

Veja a seguir um exemplo de como chamar essa API.

### <a name="request"></a>Solicitação

Este é um exemplo de solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "informationprotectionlabel_extractlabel"
}-->

```http
POST https://graph.microsoft.com/beta/informationProtection/policy/labels/extractLabel
Content-type: application/json
User-agent: ContosoLOBApp/1.0

{
    "contentInfo": {
        "@odata.type": "#microsoft.graph.contentInfo",
        "format@odata.type": "#microsoft.graph.contentFormat",
        "format": "default",
        "identifier": null,
        "state@odata.type": "#microsoft.graph.contentState",
        "state": "rest",
        "metadata@odata.type": "#Collection(microsoft.graph.keyValuePair)",
        "metadata": [
            {
                "@odata.type": "#microsoft.graph.keyValuePair",
                "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Enabled",
                "value": "True"
            },
            {
                "@odata.type": "#microsoft.graph.keyValuePair",
                "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Method",
                "value": "Standard"
            },
            {
                "@odata.type": "#microsoft.graph.keyValuePair",
                "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SetDate",
                "value": "1/1/0001 12:00:00 AM"
            },
            {
                "@odata.type": "#microsoft.graph.keyValuePair",
                "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SiteId",
                "value": "cfa4cf1d-a337-4481-aa99-19d8f3d63f7c"
            },
            {
                "@odata.type": "#microsoft.graph.keyValuePair",
                "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Name",
                "value": "Top Secret"
            },
            {
                "@odata.type": "#microsoft.graph.keyValuePair",
                "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ContentBits",
                "value": "0"
            },
            {
                "@odata.type": "#microsoft.graph.keyValuePair",
                "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ActionId",
                "value": "00000000-0000-0000-0000-000000000000"
            }
        ]
    }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/informationprotectionlabel-extractlabel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/informationprotectionlabel-extractlabel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/informationprotectionlabel-extractlabel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/informationprotectionlabel-extractlabel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/informationprotectionlabel-extractlabel-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/informationprotectionlabel-extractlabel-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.informationProtectionContentLabel"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.informationProtectionContentLabel",
    "creationDateTime": "1970-01-01T00:00:00Z",
    "assignmentMethod": "standard",
    "label": {
        "id": "722a5300-ac39-4c9a-88e3-f54c46676417",
        "name": "Top Secret",
        "description": "",
        "color": "#000000",
        "sensitivity": 13,
        "tooltip": "This information is top secret.",
        "isActive": true,
        "parent" : null
    }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "informationProtectionLabel: extractLabel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


