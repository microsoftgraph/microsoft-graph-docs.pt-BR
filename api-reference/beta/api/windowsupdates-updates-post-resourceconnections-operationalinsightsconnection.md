---
title: Criar operationalInsightsConnection
description: Crie um novo objeto operationalInsightsConnection.
author: aarononeal
ms.localizationpriority: medium
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 85990438cec500e8c7f45c08ee1fe907f1f97efc
ms.sourcegitcommit: af7a33e92d0e84e6108dd5d9466f869061ac0c97
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/19/2022
ms.locfileid: "66856493"
---
# <a name="create-operationalinsightsconnection"></a>Criar operationalInsightsConnection
Namespace: microsoft.graph.windowsUpdates

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie um novo [objeto operationalInsightsConnection](../resources/windowsupdates-operationalinsightsconnection.md) .

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
POST /admin/windows/updates/resourceConnections
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do [objeto operationalInsightsConnection](../resources/windowsupdates-operationalinsightsconnection.md) .

Você deve especificar as propriedades a seguir ao criar **um operationalInsightsConnection**.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|azureResourceGroupName|String|O nome do grupo de recursos do Azure que contém o workspace do Log Analytics.|
|azureSubscriptionId|String|A ID da assinatura do Azure que contém o workspace do Log Analytics.|
|Workspacename|String|O nome do workspace do Log Analytics.|

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código `201 Created` de resposta e um [objeto operationalInsightsConnection](../resources/windowsupdates-operationalinsightsconnection.md) no corpo da resposta.

Os seguintes erros são possíveis:

|Código da resposta|Mensagem|
|:---|:---|
|`400 Bad Request`|O workspace especificado não pôde ser vinculado. Verifique se as propriedades de chave estão corretas.|
|`403 Forbidden`|O workspace especificado não pôde ser vinculado. Verifique se a assinatura do Azure está ativa.|
|`409 Conflict`|O recurso especificado já existe.|

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.
<!-- {
  "blockType": "request",
  "name": "create_operationalInsightsConnection_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/resourceConnections
Content-Type: application/json
Content-length: 97

{
  "@odata.type": "#microsoft.graph.windowsUpdates.operationalInsightsConnection",
  "azureSubscriptionId": "322ec614-e9c2-4cd5-a55c-5711fdecf02e",
  "azureResourceGroupName": "target-resource-group",
  "workspaceName": "my-workspace"
}
```


### <a name="response"></a>Resposta
Este é um exemplo de resposta.
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsUpdates.operationalInsightsConnection"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.windowsUpdates.operationalInsightsConnection",
  "id": "85fbecb2-e407-34e9-9298-4d587857795d",
  "azureSubscriptionId": "322ec614-e9c2-4cd5-a55c-5711fdecf02e",
  "azureResourceGroupName": "target-resource-group",
  "workspaceName": "my-workspace",
  "state": "connected"
}
```