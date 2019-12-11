---
title: Atualizar Propriedadesdeviceconfigurationconflictsummary
description: Atualiza as propriedades de um objeto Propriedadesdeviceconfigurationconflictsummary.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 720b642388fd9d090af3f1a9e602ee19821a711c
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39949424"
---
# <a name="update-deviceconfigurationconflictsummary"></a>Atualizar Propriedadesdeviceconfigurationconflictsummary

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualiza as propriedades de um objeto [propriedadesdeviceconfigurationconflictsummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Application|DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [propriedadesdeviceconfigurationconflictsummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) .

A tabela a seguir mostra as propriedades que são necessárias ao criar [propriedadesdeviceconfigurationconflictsummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|conflictingDeviceConfigurations|Conjunto [settingSource](../resources/intune-deviceconfig-settingsource.md)|O conjunto de políticas em conflito com a configuração determinada|
|id|String|A ID desse conjunto de diretivas conflitantes. Esta ID é as identificações de todas as políticas no ConflictingDeviceConfigurations na ordem lexicographical separadas por sublinhados.|
|contributingSettings|Coleção de cadeias de caracteres|O conjunto de configurações em conflito com as políticas determinadas|
|deviceCheckinsImpacted|Int32|A contagem de check-ins impactados pelas políticas e configurações conflitantes|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [propriedadesdeviceconfigurationconflictsummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationConflictSummary/{deviceConfigurationConflictSummaryId}
Content-type: application/json
Content-length: 361

{
  "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
  "conflictingDeviceConfigurations": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "Id value",
      "displayName": "Display Name value"
    }
  ],
  "contributingSettings": [
    "Contributing Settings value"
  ],
  "deviceCheckinsImpacted": 6
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 410

{
  "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
  "conflictingDeviceConfigurations": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "Id value",
      "displayName": "Display Name value"
    }
  ],
  "id": "d5f22c23-2c23-d5f2-232c-f2d5232cf2d5",
  "contributingSettings": [
    "Contributing Settings value"
  ],
  "deviceCheckinsImpacted": 6
}
```





