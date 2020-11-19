---
title: Atualizar mobileAppSupersedence
description: Atualiza as propriedades de um objeto mobileAppSupersedence.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ebc3bee8a610730d2d456bd3194268f5d57263ce
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49247906"
---
# <a name="update-mobileappsupersedence"></a>Atualizar mobileAppSupersedence

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualiza as propriedades de um objeto [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementApps.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementApps.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) .

A tabela a seguir mostra as propriedades que são necessárias ao criar [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A ID da entidade de relação. Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetId|String|A ID de aplicativo do aplicativo móvel de destino. Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetDisplayName|String|O nome de exibição do aplicativo móvel de destino. Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetDisplayVersion|String|A versão de exibição do aplicativo móvel de destino. Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetPublisher|String|O fornecedor do aplicativo móvel de destino. Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)|
|targetType|[mobileAppRelationshipType](../resources/intune-apps-mobileapprelationshiptype.md)|O tipo de relação que indica se o destino é um pai ou filho. Herdado de [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md). Os valores possíveis são: `child` e `parent`.|
|supersedenceType|[mobileAppSupersedenceType](../resources/intune-apps-mobileappsupersedencetype.md)|O tipo de relação de substituição entre os aplicativos pai e filho. Os valores possíveis são: `update` e `replace`.|
|supersededAppCount|Int32|O número total de aplicativos diretamente ou indiretamente substituídos pelo aplicativo filho.|
|supersedingAppCount|Int32|O número total de aplicativos que substituem diretamente ou indiretamente o aplicativo pai.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
Content-type: application/json
Content-length: 375

{
  "@odata.type": "#microsoft.graph.mobileAppSupersedence",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "targetDisplayVersion": "Target Display Version value",
  "targetPublisher": "Target Publisher value",
  "targetType": "parent",
  "supersedenceType": "replace",
  "supersededAppCount": 2,
  "supersedingAppCount": 3
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 424

{
  "@odata.type": "#microsoft.graph.mobileAppSupersedence",
  "id": "c0254204-4204-c025-0442-25c0044225c0",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "targetDisplayVersion": "Target Display Version value",
  "targetPublisher": "Target Publisher value",
  "targetType": "parent",
  "supersedenceType": "replace",
  "supersededAppCount": 2,
  "supersedingAppCount": 3
}
```




