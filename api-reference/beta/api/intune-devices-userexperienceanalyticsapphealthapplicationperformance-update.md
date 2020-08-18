---
title: Atualizar userExperienceAnalyticsAppHealthApplicationPerformance
description: Atualiza as propriedades de um objeto userExperienceAnalyticsAppHealthApplicationPerformance.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3e845c25f1174b36941f22c249f91d365a83a590
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46793186"
---
# <a name="update-userexperienceanalyticsapphealthapplicationperformance"></a>Atualizar userExperienceAnalyticsAppHealthApplicationPerformance

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualiza as propriedades de um objeto [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementManagedDevices.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformance/{userExperienceAnalyticsAppHealthApplicationPerformanceId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) .

A tabela a seguir mostra as propriedades que são necessárias ao criar [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo do objeto de desempenho do aplicativo de análise da experiência do usuário.|
|appName|Cadeia de caracteres|O nome do aplicativo.|
|appFriendlyName|String|O nome amigável do aplicativo.|
|appPublisher|String|O fornecedor do aplicativo.|
|activeDevices|Int32|O número de dispositivos em que o aplicativo está ativo. Valores válidos-2147483648 a 2147483647|
|totalAppUsageDuration|Int32|O tempo total de uso do aplicativo em minutos. Valores válidos-2147483648 a 2147483647|
|totalAppCrashes|Int32|O número de falhas para o aplicativo. Valores válidos-2147483648 a 2147483647|
|totalAppHangs|Int32|O número de suspensões para o aplicativo. Valores válidos-2147483648 a 2147483647|
|meanTimeToFailure|Int32|O tempo médio de falha para o aplicativo em minutos. Valores válidos-2147483648 a 2147483647|
|appHealthScore|Duplo|A pontuação de integridade do aplicativo. Valores válidos-1.79769313486232 E + 308 a 1.79769313486232 E + 308|
|appHealthStatus|String|O status de integridade geral do aplicativo.|
|allOrgsHealthScore|Duplo|A pontuação de integridade mediana do aplicativo em todas as organizações. Valores válidos-1.79769313486232 E + 308 a 1.79769313486232 E + 308|
|allOrgsMeanTimeToFailure|Int32|O tempo médio de falha em todos os organizações expandidas para o aplicativo em minutos. Valores válidos-2147483648 a 2147483647|
|tenantId|String|A ID do locatário associado a este objeto de aplicativo.|
|memaTimeGenerated|String|O momento em que a agregação foi realizada no MEMA.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/intune-devices-userexperienceanalyticsapphealthapplicationperformance.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformance/{userExperienceAnalyticsAppHealthApplicationPerformanceId}
Content-type: application/json
Content-length: 591

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthApplicationPerformance",
  "appName": "App Name value",
  "appFriendlyName": "App Friendly Name value",
  "appPublisher": "App Publisher value",
  "activeDevices": 13,
  "totalAppUsageDuration": 5,
  "totalAppCrashes": 15,
  "totalAppHangs": 13,
  "meanTimeToFailure": 1,
  "appHealthScore": 4.666666666666667,
  "appHealthStatus": "App Health Status value",
  "allOrgsHealthScore": 6.0,
  "allOrgsMeanTimeToFailure": 8,
  "tenantId": "Tenant Id value",
  "memaTimeGenerated": "Mema Time Generated value"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 640

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsAppHealthApplicationPerformance",
  "id": "c7962a87-2a87-c796-872a-96c7872a96c7",
  "appName": "App Name value",
  "appFriendlyName": "App Friendly Name value",
  "appPublisher": "App Publisher value",
  "activeDevices": 13,
  "totalAppUsageDuration": 5,
  "totalAppCrashes": 15,
  "totalAppHangs": 13,
  "meanTimeToFailure": 1,
  "appHealthScore": 4.666666666666667,
  "appHealthStatus": "App Health Status value",
  "allOrgsHealthScore": 6.0,
  "allOrgsMeanTimeToFailure": 8,
  "tenantId": "Tenant Id value",
  "memaTimeGenerated": "Mema Time Generated value"
}
```



