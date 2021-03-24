---
title: Atualizar circularGeofenceManagementCondition
description: Atualize as propriedades de um objeto circularGeofenceManagementCondition.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: af17c331bde66baef8f6f5b53fa454928da06cfe
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149832"
---
# <a name="update-circulargeofencemanagementcondition"></a>Atualizar circularGeofenceManagementCondition

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de [um objeto circularGeofenceManagementCondition.](../resources/intune-fencing-circulargeofencemanagementcondition.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditions/{managementConditionId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o [objeto circularGeofenceManagementCondition.](../resources/intune-fencing-circulargeofencemanagementcondition.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo da condição de gerenciamento. Valor gerado pelo sistema atribuído quando criado. Herdado [de managementCondition](../resources/intune-fencing-managementcondition.md)|
|uniqueName|Cadeia de caracteres|Nome exclusivo para a condição de gerenciamento. Usado em expressões de condição de gerenciamento. Herdado [de managementCondition](../resources/intune-fencing-managementcondition.md)|
|displayName|Cadeia de caracteres|O nome definido pelo administrador da condição de gerenciamento. Herdado [de managementCondition](../resources/intune-fencing-managementcondition.md)|
|descrição|Cadeia de caracteres|A descrição definida pelo administrador da condição de gerenciamento. Herdado [de managementCondition](../resources/intune-fencing-managementcondition.md)|
|createdDateTime|DateTimeOffset|A hora em que a condição de gerenciamento foi criada. Lado de serviço gerado. Herdado [de managementCondition](../resources/intune-fencing-managementcondition.md)|
|modifiedDateTime|DateTimeOffset|O tempo em que a condição de gerenciamento foi modificada pela última vez. Lado do serviço atualizado. Herdado [de managementCondition](../resources/intune-fencing-managementcondition.md)|
|eTag|String|ETag da condição de gerenciamento. Lado do serviço atualizado. Herdado [de managementCondition](../resources/intune-fencing-managementcondition.md)|
|applicablePlatforms|[Coleção devicePlatformType](../resources/intune-shared-deviceplatformtype.md)|As plataformas aplicáveis para essa condição de gerenciamento. Herdado [de managementCondition](../resources/intune-fencing-managementcondition.md). Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|
|latitude|Double|Latitude em graus, entre -90 e +90 inclusive.|
|longitude|Double|Longitude em graus, entre -180 e +180 inclusive.|
|radiusInMeters|Único|Raio em metros.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto circularGeofenceManagementCondition](../resources/intune-fencing-circulargeofencemanagementcondition.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
Content-type: application/json
Content-length: 371

{
  "@odata.type": "#microsoft.graph.circularGeofenceManagementCondition",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "latitude": 2.6666666666666665,
  "longitude": 3.0,
  "radiusInMeters": 4.666666666666667
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 539

{
  "@odata.type": "#microsoft.graph.circularGeofenceManagementCondition",
  "id": "30ee27b6-27b6-30ee-b627-ee30b627ee30",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "latitude": 2.6666666666666665,
  "longitude": 3.0,
  "radiusInMeters": 4.666666666666667
}
```




