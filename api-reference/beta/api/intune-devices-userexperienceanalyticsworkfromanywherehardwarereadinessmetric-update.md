---
title: Atualizar userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric
description: Atualize as propriedades de um objeto userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 473c01d8c59912bc88880aaff42fe105b35ba234
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58265486"
---
# <a name="update-userexperienceanalyticsworkfromanywherehardwarereadinessmetric"></a>Atualizar userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de [um objeto userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric.](../resources/intune-devices-userexperienceanalyticsworkfromanywherehardwarereadinessmetric.md)

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
PATCH /deviceManagement/userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o [objeto userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric.](../resources/intune-devices-userexperienceanalyticsworkfromanywherehardwarereadinessmetric.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [o userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric](../resources/intune-devices-userexperienceanalyticsworkfromanywherehardwarereadinessmetric.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo do objeto métrico de preparação de hardware de análise de experiência do usuário.|
|totalDeviceCount|Int32|A contagem do total de dispositivos em uma organização. Valores válidos -2147483648 para 2147483647|
|upgradeEligibleDeviceCount|Int32|A contagem de dispositivos em uma organização qualificada para atualização do Windows. Valores válidos -2147483648 para 2147483647|
|ramCheckFailedPercentage|Duplo|A porcentagem de dispositivos para os quais a verificação de hardware ram falhou. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|
|storageCheckFailedPercentage|Duplo|A porcentagem de dispositivos para os quais a verificação de hardware de armazenamento falhou. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|
|processorCoreCountCheckFailedPercentage|Duplo|A porcentagem de dispositivos para os quais a contagem de núcleos de hardware do processador falhou. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|
|processorSpeedCheckFailedPercentage|Duplo|A porcentagem de dispositivos para os quais a verificação de velocidade de hardware do processador falhou. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|
|tpmCheckFailedPercentage|Duplo|A porcentagem de dispositivos para os quais a verificação de hardware TPM (Trusted Platform Module) falhou. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|
|secureBootCheckFailedPercentage|Duplo|A porcentagem de dispositivos para os quais a verificação de hardware de inicialização segura falhou. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|
|processorFamilyCheckFailedPercentage|Duplo|A porcentagem de dispositivos para os quais a família de hardware do processador falhou. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|
|processor64BitCheckFailedPercentage|Duplo|A porcentagem de dispositivos para os quais a verificação da arquitetura de hardware de 64 bits do processador falhou. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|
|osCheckFailedPercentage|Duplo|A porcentagem de dispositivos para os quais a verificação do sistema operacional falhou. Valores válidos -1,79769313486232E+308 a 1.79769313486232E+308|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric](../resources/intune-devices-userexperienceanalyticsworkfromanywherehardwarereadinessmetric.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric
Content-type: application/json
Content-length: 626

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric",
  "totalDeviceCount": 0,
  "upgradeEligibleDeviceCount": 10,
  "ramCheckFailedPercentage": 8.0,
  "storageCheckFailedPercentage": 9.3333333333333339,
  "processorCoreCountCheckFailedPercentage": 13.0,
  "processorSpeedCheckFailedPercentage": 11.666666666666666,
  "tpmCheckFailedPercentage": 8.0,
  "secureBootCheckFailedPercentage": 10.333333333333334,
  "processorFamilyCheckFailedPercentage": 12.0,
  "processor64BitCheckFailedPercentage": 11.666666666666666,
  "osCheckFailedPercentage": 7.666666666666667
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 675

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereHardwareReadinessMetric",
  "id": "6df21a06-1a06-6df2-061a-f26d061af26d",
  "totalDeviceCount": 0,
  "upgradeEligibleDeviceCount": 10,
  "ramCheckFailedPercentage": 8.0,
  "storageCheckFailedPercentage": 9.3333333333333339,
  "processorCoreCountCheckFailedPercentage": 13.0,
  "processorSpeedCheckFailedPercentage": 11.666666666666666,
  "tpmCheckFailedPercentage": 8.0,
  "secureBootCheckFailedPercentage": 10.333333333333334,
  "processorFamilyCheckFailedPercentage": 12.0,
  "processor64BitCheckFailedPercentage": 11.666666666666666,
  "osCheckFailedPercentage": 7.666666666666667
}
```




