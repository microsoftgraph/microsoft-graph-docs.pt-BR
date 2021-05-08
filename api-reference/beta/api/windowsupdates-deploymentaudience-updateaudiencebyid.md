---
title: 'deploymentAudience: updateAudienceById'
description: Atualize os membros e as coleções de exclusões de uma deploymentAudience com recursos updatableAsset do mesmo tipo.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 81404ad4807f045b75b3b161ec361f06b622f78b
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240571"
---
# <a name="deploymentaudience-updateaudiencebyid"></a>deploymentAudience: updateAudienceById
Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize os membros e as coleções de exclusões de [uma deploymentAudience](../resources/windowsupdates-deploymentaudience.md) com [recursos updatableAsset](../resources/windowsupdates-updatableasset.md) do mesmo tipo.

Adicionar um [azureADDevice](../resources/windowsupdates-azureaddevice.md) aos membros ou coleções de exclusões de um público de implantação cria automaticamente um objeto de dispositivo do Azure AD se ainda não existir.

Se o mesmo [updatableAsset](../resources/windowsupdates-updatableasset.md)  for incluído  nas exclusões e coleções de membros de uma **deploymentAudience,** a implantação não se aplicará a esse ativo.

Você também pode usar o [método updateAudience](windowsupdates-deploymentaudience-updateaudience.md) para atualizar **a deploymentAudience**.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|WindowsUpdates.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|WindowsUpdates.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/deployments/{deploymentId}/audience/updateAudienceById
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
|memberEntityType|Cadeia de caracteres|O tipo completo dos ativos atualizáveis. Os valores possíveis são: `#microsoft.graph.windowsUpdates.azureADDevice` e `#microsoft.graph.windowsUpdates.updatableAssetGroup`.|
|addMembers|Coleção de cadeias de caracteres|Lista de identificadores correspondentes aos ativos atualizáveis a adicionar como membros da audiência de implantação.|
|removeMembers|Coleção de cadeias de caracteres|Lista de identificadores correspondentes aos ativos atualizáveis a ser removidos como membros da audiência de implantação.|
|addExclusions|Coleção de cadeias de caracteres|Lista de identificadores correspondentes aos ativos atualizáveis para adicionar como exclusões do público de implantação.|
|removeExclusions|Coleção de cadeias de caracteres|Lista de identificadores correspondentes aos ativos atualizáveis para remover como exclusões do público de implantação.|



## <a name="response"></a>Resposta

Se tiver êxito, esta ação retornará um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "deploymentaudience_updateaudiencebyid"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/deployments/{deploymentId}/audience/updateAudienceById
Content-Type: application/json
Content-length: 204

{
  "memberEntityType": "String",
  "addMembers": [
    "String"
  ],
  "removeMembers": [
    "String"
  ],
  "addExclusions": [
    "String"
  ],
  "removeExclusions": [
    "String"
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/deploymentaudience-updateaudiencebyid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/deploymentaudience-updateaudiencebyid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/deploymentaudience-updateaudiencebyid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/deploymentaudience-updateaudiencebyid-java-snippets.md)]
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
```

