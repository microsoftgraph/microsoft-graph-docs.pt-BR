---
title: Criar site custodiadoSource
description: Criar um novo objeto custodiante siteSource.
author: mahage-msft
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: a5191aa1cf4dbad838cffa6dea7beb47bd0aa0de
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60986953"
---
# <a name="create-custodian-sitesource"></a>Criar site custodiadoSource

Namespace: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Criar um novo objeto [custodiante siteSource.](../resources/ediscovery-sitesource.md)

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|eDiscovery.Read.All, eDiscovery.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /compliance/ediscovery/cases/{caseId}/custodians/{custodianId}/siteSources
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornece uma representação JSON do [objeto siteSource.](../resources/ediscovery-sitesource.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [o siteSource](../resources/ediscovery-sitesource.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|site|Cadeia de caracteres|URL do site; por exemplo, `https://contoso.sharepoint.com/sites/HumanResources` .|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_sitesource_from__1"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/15d80234-8320-4f10-96d0-d98d53ffdfc9/custodians/8904528fef4d4578b44f71a80188f400/siteSources
Content-Type: application/json

{
    "site": {
        "webUrl": "https://contoso.sharepoint.com/sites/HumanResources"
    }
}

```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-sitesource-from--1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-sitesource-from--1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-sitesource-from--1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-sitesource-from--1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-sitesource-from--1-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>Resposta

**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.siteSource"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#compliance/ediscovery/cases('15d80234-8320-4f10-96d0-d98d53ffdfc9')/custodians('8904528fef4d4578b44f71a80188f400')/siteSources/$entity",
    "@odata.id": "https://graph.microsoft.com/v1.0/sites/2493b4eb-1a48-4cac-b0d0-aad05e6b9df0",
    "displayName": "Human resources site",
    "createdDateTime": "2021-08-10T18:25:48.6441363Z",
    "id": "42393244-3838-4636-3437-453030334136",
    "createdBy": {
        "user": {
            "id": "798d8d23-2087-4e03-912e-c0d9db5cb5d2",
            "displayName": null
        }
    }
}
```
