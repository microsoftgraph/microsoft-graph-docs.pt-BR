---
title: Excluir taskDefinition
description: Excluir uma definição de tarefa.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 457ebc3ba3f2e125b5d252c138ed08b28d3e0798
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516837"
---
# <a name="delete-printtaskdefinition"></a>Excluir printTaskDefinition
Namespace: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Excluir uma **tarefaDefinition**.

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
DELETE /print/taskDefinitions/{printTaskDefinitionId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "delete_printtaskdefinition"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/print/taskDefinitions/{printTaskDefinitionId}
```


### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

