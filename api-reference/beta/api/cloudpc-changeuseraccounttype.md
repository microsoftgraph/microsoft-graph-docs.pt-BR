---
title: 'cloudPC: changeUserAccountType'
description: Altere o tipo de conta do usuário em um computador cloud específico.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: e2852869f9ecd1fb2d72de17d64c97434b548f49
ms.sourcegitcommit: bfd1ab7e015ef04cb2ca3fb85d308ba2ce830a89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/19/2022
ms.locfileid: "62072776"
---
# <a name="cloudpc-changeuseraccounttype"></a>cloudPC: changeUserAccountType
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Altere o tipo de conta do usuário em um computador cloud específico.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|CloudPC.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|CloudPC.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/virtualEndpoint/cloudPCs/{cloudPCId}/changeUserAccountType
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
|userAccountType|[cloudPcUserAccountType](../resources/cloudpcorganizationsettings.md#cloudpcuseraccounttype-values)|O tipo de conta do usuário em PCs de Nuvem provisionados. Os valores possíveis são: `standardUser` `administrator` , e `unknownFutureValue` .|


## <a name="response"></a>Resposta

Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "cloudpc_changeuseraccounttype"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/cloudPCs/4b5ad5e0-6a0b-4ffc-818d-36bb23cf4dbd/changeUserAccountType
Content-Type: application/json
Content-length: 35

{
  "userAccountType": "administrator"
}
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
