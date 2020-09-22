---
title: tipo de recurso vulnerableManagedDevice
description: Esta entidade representa um dispositivo associado a uma tarefa.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e06e0a5597dc11340d6860675a15d58667fa9a48
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993613"
---
# <a name="vulnerablemanageddevice-resource-type"></a>tipo de recurso vulnerableManagedDevice

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Esta entidade representa um dispositivo associado a uma tarefa.

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar vulnerableManagedDevices](../api/intune-partnerintegration-vulnerablemanageddevice-list.md)|coleção [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md)|Listar Propriedades e relações dos objetos [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) .|
|[Obter vulnerableManagedDevice](../api/intune-partnerintegration-vulnerablemanageddevice-get.md)|[vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md)|Leia as propriedades e as relações do objeto [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) .|
|[Criar vulnerableManagedDevice](../api/intune-partnerintegration-vulnerablemanageddevice-create.md)|[vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md)|Criar um novo objeto [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) .|
|[Excluir vulnerableManagedDevice](../api/intune-partnerintegration-vulnerablemanageddevice-delete.md)|Nenhum|Exclui [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md).|
|[Atualizar vulnerableManagedDevice](../api/intune-partnerintegration-vulnerablemanageddevice-update.md)|[vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md)|Atualiza as propriedades de um objeto [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A chave da entidade e a ID do dispositivo AAD.|
|managedDeviceId|String|A ID do dispositivo gerenciado do Intune.|
|displayName|String|O nome do dispositivo.|
|lastSyncDateTime|DateTimeOffset|A data da última sincronização.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.vulnerableManagedDevice"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vulnerableManagedDevice",
  "id": "String (identifier)",
  "managedDeviceId": "String",
  "displayName": "String",
  "lastSyncDateTime": "String (timestamp)"
}
```






