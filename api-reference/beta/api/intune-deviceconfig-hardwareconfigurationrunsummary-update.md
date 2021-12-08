---
title: Atualizar hardwareConfigurationRunSummary
description: Atualize as propriedades de um objeto hardwareConfigurationRunSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5657005360e6f66d361f9490481d2b89653ea244
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61348384"
---
# <a name="update-hardwareconfigurationrunsummary"></a>Atualizar hardwareConfigurationRunSummary

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de [um objeto hardwareConfigurationRunSummary.](../resources/intune-deviceconfig-hardwareconfigurationrunsummary.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/hardwareConfigurations/{hardwareConfigurationId}/runSummary
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o [objeto hardwareConfigurationRunSummary.](../resources/intune-deviceconfig-hardwareconfigurationrunsummary.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [o hardwareConfigurationRunSummary](../resources/intune-deviceconfig-hardwareconfigurationrunsummary.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade resumo de execução de configuração de hardware. Essa propriedade é somente leitura.|
|successfulDeviceCount|Int32|Número de dispositivos para os quais o hardware foi configurado sem qualquer problema|
|failedDeviceCount|Int32|Número de dispositivos para os quais a configuração de hardware encontrou um problema|
|pendingDeviceCount|Int32|Número de dispositivos para os quais a configuração de hardware está em estado pendente|
|errorDeviceCount|Int32|Número de dispositivos para os quais o estado de configuração de hardware é erro|
|notApplicableDeviceCount|Int32|Número de dispositivos para os quais o estado de configuração de hardware não é aplicável|
|unknownDeviceCount|Int32|Número de dispositivos para os quais o estado de configuração de hardware é desconhecido|
|successfulUserCount|Int32|Número de usuários para os quais o hardware foi configurado sem qualquer problema|
|failedUserCount|Int32|Número de usuários para os quais a configuração de hardware encontrou um problema|
|pendingUserCount|Int32|Número de usuários para os quais a configuração de hardware está em estado pendente|
|errorUserCount|Int32|Número de usuários para os quais o estado de configuração de hardware é erro|
|notApplicableUserCount|Int32|Número de usuários para os quais o estado de configuração de hardware não é aplicável|
|unknownUserCount|Int32|Número de usuários para os quais o estado de configuração de hardware é desconhecido|
|lastRunDateTime|DateTimeOffset|Último tempo de execução para a configuração em todos os dispositivos|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto hardwareConfigurationRunSummary](../resources/intune-deviceconfig-hardwareconfigurationrunsummary.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/hardwareConfigurations/{hardwareConfigurationId}/runSummary
Content-type: application/json
Content-length: 469

{
  "@odata.type": "#microsoft.graph.hardwareConfigurationRunSummary",
  "successfulDeviceCount": 5,
  "failedDeviceCount": 1,
  "pendingDeviceCount": 2,
  "errorDeviceCount": 0,
  "notApplicableDeviceCount": 8,
  "unknownDeviceCount": 2,
  "successfulUserCount": 3,
  "failedUserCount": 15,
  "pendingUserCount": 0,
  "errorUserCount": 14,
  "notApplicableUserCount": 6,
  "unknownUserCount": 0,
  "lastRunDateTime": "2016-12-31T23:57:28.499537-08:00"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 518

{
  "@odata.type": "#microsoft.graph.hardwareConfigurationRunSummary",
  "id": "76b964f2-64f2-76b9-f264-b976f264b976",
  "successfulDeviceCount": 5,
  "failedDeviceCount": 1,
  "pendingDeviceCount": 2,
  "errorDeviceCount": 0,
  "notApplicableDeviceCount": 8,
  "unknownDeviceCount": 2,
  "successfulUserCount": 3,
  "failedUserCount": 15,
  "pendingUserCount": 0,
  "errorUserCount": 14,
  "notApplicableUserCount": 6,
  "unknownUserCount": 0,
  "lastRunDateTime": "2016-12-31T23:57:28.499537-08:00"
}
```




