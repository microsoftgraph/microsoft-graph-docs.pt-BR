---
title: Atualizar deviceAppManagementTask
description: Atualize as propriedades de um objeto deviceAppManagementTask.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a29705b5f420674f5f8ccc167fb05b607a4f9541
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58785819"
---
# <a name="update-deviceappmanagementtask"></a>Atualizar deviceAppManagementTask

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Atualize as propriedades de [um objeto deviceAppManagementTask.](../resources/intune-partnerintegration-deviceappmanagementtask.md)

## <a name="prerequisites"></a>Pré-requisitos
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|DeviceManagementApps.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Application|DeviceManagementApps.ReadWrite.All|

## <a name="http-request"></a>Solicitação HTTP
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Cabeçalho|Valor|
|:---|:---|
|Autorização|&lt;Token&gt; de portador obrigatório.|
|Aceitar|application/json|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON para o [objeto deviceAppManagementTask.](../resources/intune-partnerintegration-deviceappmanagementtask.md)

A tabela a seguir mostra as propriedades que são necessárias ao criar [deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md).

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A chave da entidade.|
|displayName|Cadeia de caracteres|O nome.|
|descrição|Cadeia de caracteres|A descrição.|
|createdDateTime|DateTimeOffset|A data criada.|
|dueDateTime|DateTimeOffset|A data de vencimento.|
|category|[deviceAppManagementTaskCategory](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|A categoria. Os valores possíveis são: `unknown` e `advancedThreatProtection`.|
|prioridade|[deviceAppManagementTaskPriority](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|A prioridade. Os valores possíveis são: `none`, `high`, `low`.|
|criador|Cadeia de caracteres|O endereço de email do criador.|
|creatorNotes|Cadeia de caracteres|Observações do criador.|
|assignedTo|Cadeia de caracteres|O nome ou o email do administrador ao que essa tarefa é atribuída.|
|status|[deviceAppManagementTaskStatus](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|O status. Os valores possíveis são: `unknown`, `pending`, `active`, `completed`, `rejected`.|



## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto deviceAppManagementTask](../resources/intune-partnerintegration-deviceappmanagementtask.md) atualizado no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}
Content-type: application/json
Content-length: 400

{
  "@odata.type": "#microsoft.graph.deviceAppManagementTask",
  "displayName": "Display Name value",
  "description": "Description value",
  "dueDateTime": "2017-01-01T00:02:18.1994089-08:00",
  "category": "advancedThreatProtection",
  "priority": "high",
  "creator": "Creator value",
  "creatorNotes": "Creator Notes value",
  "assignedTo": "Assigned To value",
  "status": "pending"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 508

{
  "@odata.type": "#microsoft.graph.deviceAppManagementTask",
  "id": "814545cc-45cc-8145-cc45-4581cc454581",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "dueDateTime": "2017-01-01T00:02:18.1994089-08:00",
  "category": "advancedThreatProtection",
  "priority": "high",
  "creator": "Creator value",
  "creatorNotes": "Creator Notes value",
  "assignedTo": "Assigned To value",
  "status": "pending"
}
```



