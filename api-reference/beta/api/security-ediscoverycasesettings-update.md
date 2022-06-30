---
title: Atualizar ediscoveryCaseSettings
description: Atualize as propriedades de um objeto ediscoveryCaseSettings.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 1a25eff61ef247e6a8b0b0e8aa6f0c6e367ec71b
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447265"
---
# <a name="update-ediscoverycasesettings"></a>Atualizar ediscoveryCaseSettings
Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades de [um objeto ediscoveryCaseSettings](../resources/security-ediscoverycasesettings.md) .

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|eDiscovery.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /security/cases/ediscoveryCases/{ediscoveryCaseId}/settings
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|redundancyDetection|[microsoft.graph.security.redundancyDetectionSettings](../resources/security-redundancydetectionsettings.md)|**TODO: Adicionar Descrição** Opcional.|
|topicModeling|[microsoft.graph.security.topicModelingSettings](../resources/security-topicmodelingsettings.md)|**TODO: Adicionar Descrição** Opcional.|
|Ocr|[microsoft.graph.security.ocrSettings](../resources/security-ocrsettings.md)|**TODO: Adicionar Descrição** Opcional.|



## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_ediscoverycasesettings"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/security/cases/ediscoveryCases/{ediscoveryCaseId}/settings
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.security.ediscoveryCaseSettings",
  "redundancyDetection": {
    "@odata.type": "microsoft.graph.security.redundancyDetectionSettings"
  },
  "topicModeling": {
    "@odata.type": "microsoft.graph.security.topicModelingSettings"
  },
  "ocr": {
    "@odata.type": "microsoft.graph.security.ocrSettings"
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-ediscoverycasesettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-ediscoverycasesettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-ediscoverycasesettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-ediscoverycasesettings-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-ediscoverycasesettings-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
A seguir está um exemplo da resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
