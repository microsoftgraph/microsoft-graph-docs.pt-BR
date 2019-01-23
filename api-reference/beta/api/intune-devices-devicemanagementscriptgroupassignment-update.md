---
title: Atualizar deviceManagementScriptGroupAssignment
description: Atualize as propriedades de um objeto deviceManagementScriptGroupAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bab2f5e2c363d56379e240eb6c26b95e7a0fc8b9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409976"
---
# <a name="update-devicemanagementscriptgroupassignment"></a>Atualizar deviceManagementScriptGroupAssignment

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Atualize as propriedades de um objeto [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).

|Tipo de permissão|Permissões (de privilégios máximos a mínimos)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementManagedDevices.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o objeto [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) .

A tabela a seguir mostra as propriedades que são necessárias quando você cria o [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade de atribuição de grupo de script para gerenciamento do dispositivo.|
|targetGroupId|String|A Id de grupo do Active Directory do Windows Azure Pretendemos o script.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [deviceManagementScriptGroupAssignment](../resources/intune-devices-devicemanagementscriptgroupassignment.md) no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/groupAssignments/{deviceManagementScriptGroupAssignmentId}
Content-type: application/json
Content-length: 124

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 173

{
  "@odata.type": "#microsoft.graph.deviceManagementScriptGroupAssignment",
  "id": "ecd2357d-357d-ecd2-7d35-d2ec7d35d2ec",
  "targetGroupId": "Target Group Id value"
}
```




