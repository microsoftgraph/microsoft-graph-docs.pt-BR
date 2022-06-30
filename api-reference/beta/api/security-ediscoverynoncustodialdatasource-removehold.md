---
title: 'ediscoveryNoncustodialDataSource: removeHold'
description: Inicie o processo de remoção da retenção de fontes de dados não custodiais da Descoberta Eletrônica.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: d6c78b84048cff68ed5aac4522f168daf17e50ff
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440347"
---
# <a name="ediscoverynoncustodialdatasource-removehold"></a>ediscoveryNoncustodialDataSource: removeHold
Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Inicie o processo de remoção da retenção de fontes de dados não custodiais da Descoberta Eletrônica. Depois que a operação for criada, você poderá obter o status `Location` da operação de caso recuperando o parâmetro dos cabeçalhos de resposta. O local fornece uma URL que retornará [um eDiscoveryHoldOpertaion](../resources/security-ediscoveryholdoperation.md).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|eDiscovery.Read.All, eDiscovery.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/noncustodialDataSources/removeHold
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/noncustodialDataSources/{ediscoverynoncustodialDatasourceId}/removeHold
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON dos parâmetros.

A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.

|Parâmetro|Tipo|Descrição|
|:---|:---|:---|
|ids|Coleção de cadeias de caracteres|As IDs de fontes de dados não custodiais a serem removidas da retenção. Opcional.|



## <a name="response"></a>Resposta

Se tiver êxito, esta ação retornará um código de resposta `202 Accepted`.

## <a name="examples"></a>Exemplos

### <a name="example-1-remove-hold-from-multiple-non-custodial-data-sources"></a>Exemplo 1. Remova a retenção de várias fontes de dados não custodiais.
#### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "ediscoverycustodianthis.removehold"
}
-->
``` http
POST https://graph.microsoft.com/beta/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/noncustodialdatasources/removeHold
Content-Type: application/json

{
    "ids": [
        "39333641443238353535383731453339",
        "46333131344239353834433430454335"
    ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/ediscoverycustodianthisremovehold-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/ediscoverycustodianthisremovehold-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/ediscoverycustodianthisremovehold-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/ediscoverycustodianthisremovehold-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/ediscoverycustodianthisremovehold-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Resposta
A seguir está um exemplo da resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

### <a name="example-2-remove-hold-from-a-single-non-custodial-data-source"></a>Exemplo 2. Remova a retenção de uma única fonte de dados não custodiante.
#### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "ediscoverycustodianthis.removehold"
}
-->
``` http
POST https://graph.microsoft.com/beta/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/noncustodialdatasources/39333641443238353535383731453339/removeHold
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/ediscoverycustodianthisremovehold-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/ediscoverycustodianthisremovehold-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/ediscoverycustodianthisremovehold-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/ediscoverycustodianthisremovehold-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/ediscoverycustodianthisremovehold-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>Resposta
A seguir está um exemplo da resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```
