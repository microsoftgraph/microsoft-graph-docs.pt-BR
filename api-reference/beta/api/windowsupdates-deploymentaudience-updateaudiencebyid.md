---
title: 'deploymentAudience: updateAudienceById'
description: Atualize os membros e as coleções de exclusões de uma deploymentAudience com recursos updatableAsset do mesmo tipo.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 60970c5d6b02d8c9de79e206eab2360a156c5eee
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067777"
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
|Delegado (conta corporativa ou de estudante)|WindowsUpdates.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
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
|addMembers|Coleção String|Lista de identificadores correspondentes aos ativos atualizáveis a adicionar como membros da audiência de implantação.|
|removeMembers|Coleção String|Lista de identificadores correspondentes aos ativos atualizáveis a ser removidos como membros da audiência de implantação.|
|addExclusions|Coleção String|Lista de identificadores correspondentes aos ativos atualizáveis para adicionar como exclusões do público de implantação.|
|removeExclusions|Coleção String|Lista de identificadores correspondentes aos ativos atualizáveis para remover como exclusões do público de implantação.|



## <a name="response"></a>Resposta

Se tiver êxito, esta ação retornará um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

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


### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

