---
title: Atualizar deviceComplianceScript
description: Atualize as propriedades de um objeto deviceComplianceScript.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: df6523a4173add58fc13abe1a399a3cdcdf5efa2
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61347687"
---
# <a name="update-devicecompliancescript"></a>Atualizar deviceComplianceScript

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de um [objeto deviceComplianceScript.](../resources/intune-devices-devicecompliancescript.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|DeviceManagementConfiguration.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o [objeto deviceComplianceScript.](../resources/intune-devices-devicecompliancescript.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo do script de conformidade do dispositivo|
|publicador|String|Nome do editor de scripts de conformidade do dispositivo|
|versão|String|Versão do script de conformidade do dispositivo|
|displayName|String|Nome do script de conformidade do dispositivo|
|descrição|String|Descrição do script de conformidade do dispositivo|
|detectionScriptContent|Binária|Todo o conteúdo do script do powershell de detecção|
|createdDateTime|DateTimeOffset|O data/hora de quando o script de conformidade do dispositivo foi criado. Essa propriedade é somente leitura.|
|lastModifiedDateTime|DateTimeOffset|O data/hora de quando o script de conformidade do dispositivo foi modificado. Essa propriedade é somente leitura.|
|runAsAccount|[runAsAccountType](../resources/intune-shared-runasaccounttype.md)|Indica o tipo de contexto de execução. Os valores possíveis são: `system` e `user`.|
|enforceSignatureCheck|Booliano|Indicar se a assinatura de script precisa ser verificada|
|runAs32Bit|Booliano|Indicar se os scripts do PowerShell devem ser executados como 32 bits|
|roleScopeTagIds|Coleção de cadeias de caracteres|Lista de IDs de marca de escopo para o script de conformidade do dispositivo|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceComplianceScript](../resources/intune-devices-devicecompliancescript.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceComplianceScripts/{deviceComplianceScriptId}
Content-type: application/json
Content-length: 420

{
  "@odata.type": "#microsoft.graph.deviceComplianceScript",
  "publisher": "Publisher value",
  "version": "Version value",
  "displayName": "Display Name value",
  "description": "Description value",
  "detectionScriptContent": "ZGV0ZWN0aW9uU2NyaXB0Q29udGVudA==",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 592

{
  "@odata.type": "#microsoft.graph.deviceComplianceScript",
  "id": "14e72a7b-2a7b-14e7-7b2a-e7147b2ae714",
  "publisher": "Publisher value",
  "version": "Version value",
  "displayName": "Display Name value",
  "description": "Description value",
  "detectionScriptContent": "ZGV0ZWN0aW9uU2NyaXB0Q29udGVudA==",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "runAsAccount": "user",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




