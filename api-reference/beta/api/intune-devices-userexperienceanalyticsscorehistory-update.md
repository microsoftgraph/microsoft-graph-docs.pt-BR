---
title: Atualizar userExperienceAnalyticsScoreHistory
description: Atualize as propriedades de um objeto userExperienceAnalyticsScoreHistory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c6a40bf69f1b387c14657b2ae6e307d8b1a6d6a2
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688840"
---
# <a name="update-userexperienceanalyticsscorehistory"></a>Atualizar userExperienceAnalyticsScoreHistory

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de [um objeto userExperienceAnalyticsScoreHistory.](../resources/intune-devices-userexperienceanalyticsscorehistory.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementManagedDevices.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/userExperienceAnalyticsScoreHistory/{userExperienceAnalyticsScoreHistoryId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o [objeto userExperienceAnalyticsScoreHistory.](../resources/intune-devices-userexperienceanalyticsscorehistory.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [o userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo do processo de inicialização do dispositivo de análise de experiência do usuário.|
|startupDateTime|DateTimeOffset|A data de inicialização do dispositivo de análise de experiência do usuário.|
|overallScore|Int32|Pontuação geral da análise de experiência do usuário. A pontuação estará no intervalo de 0 a 100, 100 é a pontuação ideal. Valores válidos de 0 a 100|
|startupScore|Int32|Pontuação de inicialização do dispositivo de análise de experiência do usuário. A pontuação estará no intervalo de 0 a 100, 100 é a pontuação ideal.|
|coreBootScore|Int32|A pontuação de inicialização principal do dispositivo de análise de experiência do usuário. A pontuação estará no intervalo de 0 a 100, 100 é a pontuação ideal.|
|coreSigninScore|Int32|A pontuação de entrada principal do dispositivo de análise de experiência do usuário. A pontuação estará no intervalo de 0 a 100, 100 é a pontuação ideal.|
|recommendedSoftwareScore|Int32|A pontuação de entrada principal do dispositivo de análise de experiência do usuário. A pontuação estará no intervalo de 0 a 100, 100 é a pontuação ideal.|
|appHealthOverallScore|Int32|A pontuação geral de saúde geral do aplicativo de análise de experiência do usuário.|
|batteryHealthScore|Int32|A pontuação de saúde da bateria de análise de experiência do usuário.|
|startupTotalDevices|Int32|A contagem total de dispositivos do desempenho de inicialização da categoria de análise de experiência do usuário.|
|recommendedSoftwareTotalDevices|Int32|A contagem total de dispositivos do software recomendado da categoria de análise de experiência do usuário.|
|appHealthTotalDevices|Int32|A contagem total de dispositivos da saúde do aplicativo de categoria de análise de experiência do usuário.|
|batteryHealthTotalDevices|Int32|A contagem total de dispositivos da saúde da bateria da categoria de análise de experiência do usuário.|
|restartScore|Int32|Reinicie a pontuação. A pontuação estará no intervalo de 0 a 100, 100 é a pontuação ideal, 0 indica reinicializações excessivas. Valores válidos de 0 a 9999999|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userExperienceAnalyticsScoreHistory](../resources/intune-devices-userexperienceanalyticsscorehistory.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsScoreHistory/{userExperienceAnalyticsScoreHistoryId}
Content-type: application/json
Content-length: 485

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsScoreHistory",
  "startupDateTime": "2017-01-01T00:03:13.1084278-08:00",
  "overallScore": 12,
  "startupScore": 12,
  "coreBootScore": 13,
  "coreSigninScore": 15,
  "recommendedSoftwareScore": 8,
  "appHealthOverallScore": 5,
  "batteryHealthScore": 2,
  "startupTotalDevices": 3,
  "recommendedSoftwareTotalDevices": 15,
  "appHealthTotalDevices": 5,
  "batteryHealthTotalDevices": 9,
  "restartScore": 12
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 534

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsScoreHistory",
  "id": "d15e3ba8-3ba8-d15e-a83b-5ed1a83b5ed1",
  "startupDateTime": "2017-01-01T00:03:13.1084278-08:00",
  "overallScore": 12,
  "startupScore": 12,
  "coreBootScore": 13,
  "coreSigninScore": 15,
  "recommendedSoftwareScore": 8,
  "appHealthOverallScore": 5,
  "batteryHealthScore": 2,
  "startupTotalDevices": 3,
  "recommendedSoftwareTotalDevices": 15,
  "appHealthTotalDevices": 5,
  "batteryHealthTotalDevices": 9,
  "restartScore": 12
}
```



