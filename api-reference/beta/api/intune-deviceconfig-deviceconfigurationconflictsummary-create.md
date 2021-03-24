---
title: Criar deviceConfigurationConflictSummary
description: Crie um novo objeto deviceConfigurationConflictSummary.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fbb45d16011d1af458ff68fa465a1d9de5007afa
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131740"
---
# <a name="create-deviceconfigurationconflictsummary"></a>Criar deviceConfigurationConflictSummary

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Crie um novo [objeto deviceConfigurationConflictSummary.](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md)

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
POST /deviceManagement/deviceConfigurationConflictSummary
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto deviceConfigurationConflictSummary.

A tabela a seguir mostra as propriedades necessárias ao criar deviceConfigurationConflictSummary.

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|conflictingDeviceConfigurations|Conjunto [settingSource](../resources/intune-deviceconfig-settingsource.md)|O conjunto de políticas em conflito com a configuração determinada|
|id|Cadeia de caracteres|A id desse conjunto de políticas conflitantes. Esta id é a ids de todas as políticas em ConflictingDeviceConfigurations em ordem lexicographical separada por sublinhados.|
|contributingSettings|Coleção de cadeias de caracteres|O conjunto de configurações em conflito com as políticas determinadas|
|deviceCheckinsImpacted|Int32|A contagem de checkins afetados pelas políticas e configurações conflitantes|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto deviceConfigurationConflictSummary](../resources/intune-deviceconfig-deviceconfigurationconflictsummary.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurationConflictSummary
Content-type: application/json
Content-length: 398

{
  "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
  "conflictingDeviceConfigurations": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "Id value",
      "displayName": "Display Name value",
      "sourceType": "deviceIntent"
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
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 447

{
  "@odata.type": "#microsoft.graph.deviceConfigurationConflictSummary",
  "conflictingDeviceConfigurations": [
    {
      "@odata.type": "microsoft.graph.settingSource",
      "id": "Id value",
      "displayName": "Display Name value",
      "sourceType": "deviceIntent"
    }
  ],
  "id": "d5f22c23-2c23-d5f2-232c-f2d5232cf2d5",
  "contributingSettings": [
    "Contributing Settings value"
  ],
  "deviceCheckinsImpacted": 6
}
```




