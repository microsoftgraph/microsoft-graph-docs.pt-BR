---
title: Atualizar userExperienceAnalyticsImpactingProcess
description: Atualize as propriedades de um objeto userExperienceAnalyticsImpactingProcess.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 18be2d4556c454d387418a0ba434aa51bc0ea7e3
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50445703"
---
# <a name="update-userexperienceanalyticsimpactingprocess"></a>Atualizar userExperienceAnalyticsImpactingProcess

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de [um objeto userExperienceAnalyticsImpactingProcess.](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
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
PATCH /deviceManagement/userExperienceAnalyticsImpactingProcess/{userExperienceAnalyticsImpactingProcessId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o [objeto userExperienceAnalyticsImpactingProcess.](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [o userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo da entidade de processo de análise de experiência do usuário.|
|deviceId|Cadeia de caracteres|O identificador exclusivo do dispositivo afetado.|
|category|String|A categoria do processo de impacto.|
|processName|String|O nome do processo.|
|descrição|String|A descrição do processo.|
|publicador|String|O editor do processo.|
|impactValue|Duplo|O valor de impacto do processo. Valores válidos de 0 a 1,79769313486232E+308|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsImpactingProcess/{userExperienceAnalyticsImpactingProcessId}
Content-type: application/json
Content-length: 300

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsImpactingProcess",
  "deviceId": "Device Id value",
  "category": "Category value",
  "processName": "Process Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "impactValue": 3.6666666666666665
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 349

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsImpactingProcess",
  "id": "faefd665-d665-faef-65d6-effa65d6effa",
  "deviceId": "Device Id value",
  "category": "Category value",
  "processName": "Process Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "impactValue": 3.6666666666666665
}
```




