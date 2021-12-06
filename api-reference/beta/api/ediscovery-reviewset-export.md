---
title: 'reviewSet: export'
description: Inicie uma exportação de um reviewSet.
author: mahage-msft
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 577f219e004b790ab144715dbcccaf5c29e94492
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60998644"
---
# <a name="reviewset-export"></a>reviewSet: export

Namespace: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Iniciar uma exportação de um **reviewSet**.  Para obter detalhes, [consulte Exportar documentos de um conjunto de revisão em Advanced eDiscovery](/microsoft-365/compliance/export-documents-from-review-set).

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
POST /compliance/ediscovery/cases/{caseId}/reviewsets/{reviewsetId}/export
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, fornece uma representação JSON dos parâmetros.

A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.

|Parâmetro|Tipo|Descrição|
|:---|:---|:---|
|outputName|Cadeia de caracteres| Nome da exportação. Obrigatório. |
|description|String| Descrição da exportação |
|azureBlobContainer|String| Ao exportar para sua própria conta de armazenamento do Azure, essa é a URL do contêiner. |
|azureBlobToken|Cadeia de caracteres| Ao exportar para sua própria conta de armazenamento do Azure, o token SAS para a URL do contêiner. |
|exportOptions| [microsoft.graph.ediscovery.exportOptions](../resources/ediscovery-caseexportoperation.md#exportoptions-values) |Especifica opções que controlam o formato da exportação. Os valores possíveis são: `originalFiles`, `text`, `pdfReplacement`, `fileInfo`, `tags`.|
|exportStructure|[microsoft.graph.ediscovery.exportFileStructure](../resources/ediscovery-caseexportoperation.md#exportfilestructure-values)| Opções que controlam a estrutura do arquivo e o empacotamento da exportação. Os valores possíveis são: `none`, `directory`, `pst`.|

## <a name="response"></a>Resposta

Se a exportação for iniciada com êxito, essa ação retornará um `202 Accepted` código de resposta. A resposta também conterá um header, que contém o local `Location` [do caseExportOperation](../resources/ediscovery-caseexportoperation.md) que foi criado para manipular a exportação. Verifique o status da operação de exportação fazendo uma solicitação GET para o local, quando concluído com êxito, o [status](../resources/ediscovery-caseoperation.md#caseoperationstatus-values) mudará para `succeeded` .

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reviewset_export"
}
-->

``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/99e865fc-e29f-479a-ba83-9e58eb017103/reviewsets/e44ac2cb-f8b4-4fd8-aa1c-1391b46ba9cc/export
Content-Type: application/json

{
  "outputName": "2020-12-06 Contoso investigation export",
  "description": "Export for the Contoso investigation",
  "exportOptions": "originalFiles,fileInfo,tags",
  "exportStructure": "directory"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reviewset-export-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reviewset-export-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reviewset-export-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reviewset-export-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/reviewset-export-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 202 Accepted
cache-control: no-cache,
client-request-id: 3ec98906-7187-927e-5203-2ed4533175c6,
location: https://graph.microsoft.com/beta/compliance/ediscovery/cases('5b840b94-f821-4c4a-8cad-3a90062bf51a')/operations('2ad2da7c7dbb404abfbbb28b7b6babd6'),
request-id: 9e6b9230-113c-49de-8f7d-ecb90d35b0de
```
