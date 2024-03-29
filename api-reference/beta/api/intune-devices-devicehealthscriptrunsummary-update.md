---
title: Atualizar deviceHealthScriptRunSummary
description: Atualize as propriedades de um objeto deviceHealthScriptRunSummary.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7c3a0308960836b8b12e65cc7ab6b8db72174d53
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59121974"
---
# <a name="update-devicehealthscriptrunsummary"></a>Atualizar deviceHealthScriptRunSummary

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de [um objeto deviceHealthScriptRunSummary.](../resources/intune-devices-devicehealthscriptrunsummary.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/runSummary
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o [objeto deviceHealthScriptRunSummary.](../resources/intune-devices-devicehealthscriptrunsummary.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade resumo do script de saúde do dispositivo. Essa propriedade é somente leitura.|
|noIssueDetectedDeviceCount|Int32|Número de dispositivos para os quais o script de detecção não encontrou um problema e o dispositivo está saudável|
|issueDetectedDeviceCount|Int32|Número de dispositivos para os quais o script de detecção encontrou um problema|
|detectionScriptErrorDeviceCount|Int32|Número de dispositivos nos quais a execução do script de detecção encontrou um erro e não foi concluída|
|detectionScriptPendingDeviceCount|Int32|Número de dispositivos que ainda não executaram a versão mais recente do script de saúde do dispositivo|
|detectionScriptNotApplicableDeviceCount|Int32|Número de dispositivos para os quais o script de detecção não foi aplicável|
|issueRemediatedDeviceCount|Int32|Número de dispositivos para os quais o script de correção foi capaz de resolver o problema detectado|
|remediationSkippedDeviceCount|Int32|Número de dispositivos para os quais a correção foi ignorada|
|issueReoccurredDeviceCount|Int32|Número de dispositivos para os quais o script de correção foi executado com êxito, mas não conseguiu resolver o problema detectado|
|remediationScriptErrorDeviceCount|Int32|Número de dispositivos para os quais a execução do script de correção encontrou um erro e não foi concluída|
|lastScriptRunDateTime|DateTimeOffset|Tempo de última duração do script em todos os dispositivos|
|issueRemediatedCumulativeDeviceCount|Int32|Número de dispositivos que foram remediados nos últimos 30 dias|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceHealthScriptRunSummary](../resources/intune-devices-devicehealthscriptrunsummary.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/runSummary
Content-type: application/json
Content-length: 543

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunSummary",
  "noIssueDetectedDeviceCount": 10,
  "issueDetectedDeviceCount": 8,
  "detectionScriptErrorDeviceCount": 15,
  "detectionScriptPendingDeviceCount": 1,
  "detectionScriptNotApplicableDeviceCount": 7,
  "issueRemediatedDeviceCount": 10,
  "remediationSkippedDeviceCount": 13,
  "issueReoccurredDeviceCount": 10,
  "remediationScriptErrorDeviceCount": 1,
  "lastScriptRunDateTime": "2017-01-01T00:01:17.4310553-08:00",
  "issueRemediatedCumulativeDeviceCount": 4
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 592

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunSummary",
  "id": "8221b043-b043-8221-43b0-218243b02182",
  "noIssueDetectedDeviceCount": 10,
  "issueDetectedDeviceCount": 8,
  "detectionScriptErrorDeviceCount": 15,
  "detectionScriptPendingDeviceCount": 1,
  "detectionScriptNotApplicableDeviceCount": 7,
  "issueRemediatedDeviceCount": 10,
  "remediationSkippedDeviceCount": 13,
  "issueReoccurredDeviceCount": 10,
  "remediationScriptErrorDeviceCount": 1,
  "lastScriptRunDateTime": "2017-01-01T00:01:17.4310553-08:00",
  "issueRemediatedCumulativeDeviceCount": 4
}
```



