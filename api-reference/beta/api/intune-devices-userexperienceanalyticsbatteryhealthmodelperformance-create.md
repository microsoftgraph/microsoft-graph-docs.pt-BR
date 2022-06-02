---
title: Criar userExperienceAnalyticsBatteryHealthModelPerformance
description: Crie um novo objeto userExperienceAnalyticsBatteryHealthModelPerformance.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cbe1f1ff409c602ccf578003ee0bf75a8a5b73a8
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2022
ms.locfileid: "65857817"
---
# <a name="create-userexperienceanalyticsbatteryhealthmodelperformance"></a>Criar userExperienceAnalyticsBatteryHealthModelPerformance

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
|Application|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsBatteryHealthModelPerformance
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto userExperienceAnalyticsBatteryHealthModelPerformance.

A tabela a seguir mostra as propriedades que são necessárias ao criar userExperienceAnalyticsBatteryHealthModelPerformance.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo do objeto de desempenho do modelo de integridade da bateria de análise da experiência do usuário.|
|activeDevices|Int32|Número de dispositivos ativos para esse modelo. Valores válidos -2147483648 para 2147483647|
|modelo|String|O nome do modelo do dispositivo.|
|fabricante|String|Nome do fabricante do dispositivo.|
|averageMaxCapacityPercentage|Int32|A média da capacidade máxima para todos os dispositivos de um determinado modelo. A capacidade máxima mede a carga total versus a capacidade de design das baterias de um dispositivo.. Valores válidos -2147483648 para 2147483647|
|averageEstimatedRuntimeInMinutes|Int32|A média dos runtimes estimados com custo total para todos os dispositivos de um determinado modelo. Unidade em minutos. Valores válidos -2147483648 para 2147483647|
|averageBatteryAgeInDays|Int32|A média da duração da bateria para todos os dispositivos de um determinado modelo em um locatário. Unidade em dias. Valores válidos -2147483648 para 2147483647|
|modelBatteryHealthScore|Int32|Uma média ponderada da pontuação máxima de capacidade de um modelo e da pontuação de estimativa de runtime. Os valores variam de 0 a 100. Valores válidos -2147483648 para 2147483647|



## <a name="response"></a>Resposta
Se tiver êxito, este `201 Created` método retornará um código de resposta e um [objeto userExperienceAnalyticsBatteryHealthModelPerformance](../resources/intune-devices-userexperienceanalyticsbatteryhealthmodelperformance.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsBatteryHealthModelPerformance
Content-type: application/json
Content-length: 333

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthModelPerformance",
  "activeDevices": 13,
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "averageMaxCapacityPercentage": 12,
  "averageEstimatedRuntimeInMinutes": 0,
  "averageBatteryAgeInDays": 7,
  "modelBatteryHealthScore": 7
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 382

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBatteryHealthModelPerformance",
  "id": "0850afa4-afa4-0850-a4af-5008a4af5008",
  "activeDevices": 13,
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "averageMaxCapacityPercentage": 12,
  "averageEstimatedRuntimeInMinutes": 0,
  "averageBatteryAgeInDays": 7,
  "modelBatteryHealthScore": 7
}
```




