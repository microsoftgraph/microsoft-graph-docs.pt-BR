---
title: 'workbook: tableRowOperationResult'
description: Parte de uma solicitação criar tableRow assíncrona.
author: lumine2008
ms.localizationpriority: medium
ms.prod: excel
doc_type: apiPageType
ms.openlocfilehash: 4190c0fa22c1f9bb1c1918ecdf990017223a5753
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62121508"
---
# <a name="workbook-tablerowoperationresult"></a>workbook: tableRowOperationResult
Namespace: microsoft.graph

Esta função é a última de uma série de etapas para criar um recurso [workbookTableRow](../resources/workbooktablerow.md) de forma assíncrona.

Uma prática prática para criar várias linhas de tabela é em lotá-las em lotes em uma operação [de criação de tableRow](./table-post-rows.md) e realizar a operação de forma assíncrona.

Uma solicitação assíncrona para criar linhas de tabela envolve as seguintes etapas:
1. Emitir uma solicitação [Criar tableRow](./table-post-rows.md) assíncrona e obter a URL de consulta retornada no `Location` header de resposta.
2. Use a URL de consulta retornada da etapa 1 para emitir a solicitação [Get workbookOperation](./workbookoperation-get.md) e obter a ID da operação para a etapa 3. 
    Como alternativa, por conveniência, depois de obter um resultado operationStatus, você pode obter a URL de consulta da `succeeded`  **propriedade resourceLocation** da [workbookOperation](../resources/workbookoperation.md) retornada na resposta e aplicar a URL de consulta à etapa 3. 
3. Use a URL de consulta retornada da etapa 2 como a URL de solicitação GET para esta função **tableRowOperationResult**. Uma chamada de função bem-sucedida retorna as novas linhas de tabela em um [recurso workbookTableRow.](../resources/workbooktablerow.md)

Essa função não fará nada se for chamada independentemente.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|Files.ReadWrite|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/drive/items/{id}/workbook/tableRowOperationResult(key={operation-id})
GET /me/drive/root:/{item-path}:/workbook/tableRowOperationResult(key={operation-id})
```

## <a name="function-parameters"></a>Parâmetros de função
A URL de solicitação requer o parâmetro de consulta a seguir. 

|Parâmetro|Tipo|Descrição|
|:---|:---|:---|
|key|Cadeia de caracteres|A **operationId** fornecida na **resposta workbookOperation** retornada na solicitação [Get workbookOperation](./workbookoperation-get.md) anterior.|


## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
| Workbook-Session-Id  | ID da sessão da workbook que determina se as alterações são persistentes. Opcional.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, essa função retornará um código de resposta e um `200 OK` [objeto workbookTableRow](../resources/workbooktablerow.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

O exemplo a seguir mostra uma solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["0195cfac-bd22-4f91-b276-dece0aa2378b"],
  "name": "workbook_tablerowoperationresult"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/drive/items/01CCETFLK7GVZTZHSQNRD2AEI5XWTCU6FJ/workbook/tableRowOperationResult(key='0195cfac-bd22-4f91-b276-dece0aa2378b')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/workbook-tablerowoperationresult-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/workbook-tablerowoperationresult-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/workbook-tablerowoperationresult-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/workbook-tablerowoperationresult-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta

Este é um exemplo de resposta.

>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookTableRow"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "index": 99,
  "values": "[[1, 2, 3]]"
}
```
