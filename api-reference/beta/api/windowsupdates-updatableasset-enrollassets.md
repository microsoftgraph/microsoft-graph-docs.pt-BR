---
title: 'updatableAsset: enrollAssets'
description: Registrar recursos updatableAsset no gerenciamento de atualizações pelo serviço de implantação.
author: Alice-at-Microsoft
ms.localizationpriority: medium
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 7ae0848507f6d46edfea6d7faf47d4083eed43a1
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2021
ms.locfileid: "60891085"
---
# <a name="updatableasset-enrollassets"></a>updatableAsset: enrollAssets
Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Registrar [recursos updatableAsset](../resources/windowsupdates-updatableasset.md) no gerenciamento de atualizações pelo serviço de implantação.

Você pode registrar um [recurso do azureADDevice](../resources/windowsupdates-azureaddevice.md) no gerenciamento de atualizações, mas pode não registrar um [UpdateableAssetGroup](../resources/windowsupdates-updatableassetgroup.md) no gerenciamento de atualizações.

Registrar um dispositivo do Azure AD no gerenciamento de atualizações cria automaticamente um **objeto azureADDevice** se ele ainda não existir.

Você também pode usar o método [enrollAssetsById para](windowsupdates-updatableasset-enrollassetsbyid.md) registrar ativos.

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
POST /admin/windows/updates/updatableAssets/enrollAssets
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
|updateCategory|microsoft.graph.windowsUpdates.updateCategory|A categoria de atualizações para o serviço gerenciar. Oferece suporte a um subconjunto dos valores **para updateCategory**. Os valores possíveis são: `feature` e `unknownFutureValue`.|
|assets|[coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)|Lista de **recursos updatableAsset** para se inscrever no gerenciamento de atualizações pelo serviço para a **atualização determinadaCategory**.|

## <a name="response"></a>Resposta

Se tiver êxito, esta ação retornará um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "updatableasset_enrollassets"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/enrollAssets
Content-Type: application/json

{
  "updateCategory": "String",
  "assets": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "String (identifier)"
    }
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/updatableasset-enrollassets-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/updatableasset-enrollassets-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/updatableasset-enrollassets-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/updatableasset-enrollassets-java-snippets.md)]
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

