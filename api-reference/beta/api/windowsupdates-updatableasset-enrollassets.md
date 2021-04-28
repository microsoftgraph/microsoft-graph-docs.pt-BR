---
title: 'updatableAsset: enrollAssets'
description: Registrar recursos updatableAsset no gerenciamento de atualizações pelo serviço de implantação.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 2b488eaaa70ba0b04a440aabcde0d759ad6e8d36
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067272"
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
|updateCategory|microsoft.graph.windowsUpdates.updateCategory|A categoria de atualizações para o serviço gerenciar. Oferece suporte a um subconjunto dos valores **para updateCategory**. Os valores possíveis são: `feature` .|
|assets|[coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)|Lista de **recursos updatableAsset** para se inscrever no gerenciamento de atualizações pelo serviço para a **atualização determinadaCategory**.|

## <a name="response"></a>Resposta

Se tiver êxito, esta ação retornará um código de resposta `202 Accepted`. Não retorna nada no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
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


### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```

