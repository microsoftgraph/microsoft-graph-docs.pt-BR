---
title: Atualizar printTaskDefinition
description: Atualize uma definição de tarefa.
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 61c5dc81551f5f72ca4dfd4108ba950dc9dfd491
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2021
ms.locfileid: "60945912"
---
# <a name="update-printtaskdefinition"></a>Atualizar printTaskDefinition

Namespace: microsoft.graph

Atualize uma definição de tarefa.

Para obter detalhes sobre como usar essa API para adicionar suporte à impressão pull à Impressão Universal, consulte [Extending Universal Print to support pull printing](/graph/universal-print-concept-overview#extending-universal-print-to-support-pull-printing).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa.

|Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:---------------|:--------------------------------------------|
|Delegado (conta corporativa ou de estudante)| Sem suporte. |
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo| PrintTaskDefinition.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /print/taskDefinitions/{printTaskDefinitionId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece os valores para os campos [printTaskDefinition](../resources/printtaskdefinition.md) relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|displayName|Cadeia de caracteres|O nome da **printTaskDefinition**.|
|createdBy|Cadeia de caracteres|Informações sobre o aplicativo que criou a definição de tarefa. Somente a `createdBy.displayName` propriedade pode ser atualizada.|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto printTaskDefinition](../resources/printtaskdefinition.md) atualizado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_printtaskdefinition"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/print/taskDefinitions/{printTaskDefinitionId}
Content-Type: application/json

{
  "displayName": "Test TaskDefinitionName",
  "createdBy": {
    "displayName": "Requesting App Display Name"
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-printtaskdefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-printtaskdefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-printtaskdefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-printtaskdefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta
**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printTaskDefinition"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/taskDefinitions/$entity",
  "id": "fab143fd-ee61-4358-8558-2c7dee953982",
  "displayName": "Test TaskDefinitionName",
  "createdBy": {
    "appId" : "479688a0-cc3a-4993-ab24-54c7c80b047e",
    "displayName": "Requesting App Display Name"
  }
}
```

