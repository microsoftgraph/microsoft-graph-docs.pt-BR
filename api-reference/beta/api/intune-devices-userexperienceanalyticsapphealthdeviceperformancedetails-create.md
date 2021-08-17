---
title: Criar userExperienceAnalyticsAppHealthDevicePerformanceDetails
description: Crie um novo objeto userExperienceAnalyticsAppHealthDevicePerformanceDetails.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4c0ee58fd0b836076b8f2f946232a09dcfe38790
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58262797"
---
# <a name="create-userexperienceanalyticsapphealthdeviceperformancedetails"></a>Criar userExperienceAnalyticsAppHealthDevicePerformanceDetails

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto userExperienceAnalyticsAppHealthDevicePerformanceDetails.](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsAppHealthDevicePerformanceDetails
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto userExperienceAnalyticsAppHealthDevicePerformanceDetails.

A tabela a seguir mostra as propriedades que são necessárias ao criar o userExperienceAnalyticsAppHealthDevicePerformanceDetails.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo do objeto de desempenho do dispositivo de análise de experiência do usuário.|
|eventDateTime|DateTimeOffset|A hora em que o evento ocorreu.|
|eventType|Cadeia de caracteres|O tipo do evento.|
|appDisplayName|Cadeia de caracteres|O nome amigável do aplicativo para o qual o evento ocorreu.|
|appPublisher|Cadeia de caracteres|O editor do aplicativo.|
|appVersion|Cadeia de caracteres|A versão do aplicativo.|
|deviceId|Cadeia de caracteres|A id do dispositivo.|
|deviceDisplayName|Cadeia de caracteres|O nome do dispositivo.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthDevicePerformanceDetails
Content-type: application/json
Content-length: 405

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformanceDetails",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "eventType": "Event Type value",
  "appDisplayName": "App Display Name value",
  "appPublisher": "App Publisher value",
  "appVersion": "App Version value",
  "deviceId": "Device Id value",
  "deviceDisplayName": "Device Display Name value"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 454

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthDevicePerformanceDetails",
  "id": "bc8c5273-5273-bc8c-7352-8cbc73528cbc",
  "eventDateTime": "2016-12-31T23:59:23.3984029-08:00",
  "eventType": "Event Type value",
  "appDisplayName": "App Display Name value",
  "appPublisher": "App Publisher value",
  "appVersion": "App Version value",
  "deviceId": "Device Id value",
  "deviceDisplayName": "Device Display Name value"
}
```




