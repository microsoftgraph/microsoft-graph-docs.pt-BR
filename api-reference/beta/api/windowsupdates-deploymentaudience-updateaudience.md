---
title: 'deploymentAudience: updateAudience'
description: Atualize os membros e as coleções de exclusões de uma deploymentAudience.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 23fe655e076987ffb33591eb8aaa1600ed4a8fa4
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351122"
---
# <a name="deploymentaudience-updateaudience"></a>deploymentAudience: updateAudience

Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualizar os membros e coleções de exclusões de [uma deploymentAudience](../resources/windowsupdates-deploymentaudience.md).

Adicionar um [azureADDevice](../resources/windowsupdates-azureaddevice.md) aos membros ou coleções de exclusões de um público de implantação cria automaticamente um objeto de dispositivo do Azure AD, se ainda não existir.

Se o mesmo [updatableAsset](../resources/windowsupdates-updatableasset.md)  for incluído  nas exclusões e coleções de membros de uma **deploymentAudience,** a implantação não se aplicará a esse ativo.

Se todos **os objetos updateableAsset** são do mesmo tipo, você também pode usar o método [updateAudienceById](windowsupdates-deploymentaudience-updateaudiencebyid.md) para atualizar **a deploymentAudience**.

> [!NOTE]
> Essa API tem um [problema conhecido relacionado](/Graph/known-issues#accessing-and-updating-deployment-audiences) a implantações criadas por meio do Intune.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|WindowsUpdates.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Application|WindowsUpdates.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/deployments/{deploymentId}/audience/updateAudience
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
|addMembers|[coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)|Lista de [recursos updatableAsset](../resources/windowsupdates-updatableasset.md) a adicionar como membros da audiência de implantação.|
|removeMembers|[coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)|Lista de ativos atualizáveis para remover como membros da audiência de implantação.|
|addExclusions|[coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)|Lista de ativos atualizáveis para adicionar como exclusões da audiência de implantação.|
|removeExclusions|[coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)|Lista de ativos atualizáveis para remover como exclusões da audiência de implantação.|



## <a name="response"></a>Resposta

Se tiver êxito, esta ação retornará um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "deploymentaudience_updateaudience"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/deployments/{deploymentId}/audience/updateAudience
Content-Type: application/json
Content-length: 599

{
  "addMembers": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.updatableAsset",
      "id": "String (identifier)"
    }
  ],
  "removeMembers": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.updatableAsset",
      "id": "String (identifier)"
    }
  ],
  "addExclusions": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.updatableAsset",
      "id": "String (identifier)"
    }
  ],
  "removeExclusions": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.updatableAsset",
      "id": "String (identifier)"
    }
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/deploymentaudience-updateaudience-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/deploymentaudience-updateaudience-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/deploymentaudience-updateaudience-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/deploymentaudience-updateaudience-java-snippets.md)]
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

