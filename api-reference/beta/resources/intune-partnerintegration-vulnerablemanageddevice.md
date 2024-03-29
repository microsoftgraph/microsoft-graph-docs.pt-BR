---
title: tipo de recurso vulnerableManagedDevice
description: Essa entidade representa um dispositivo associado a uma tarefa.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2e6b498248d3143c6313ba97b839f7f6918a3af1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59068645"
---
# <a name="vulnerablemanageddevice-resource-type"></a>tipo de recurso vulnerableManagedDevice

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Essa entidade representa um dispositivo associado a uma tarefa.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar vulnerableManagedDevices](../api/intune-partnerintegration-vulnerablemanageddevice-list.md)|[coleção vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md)|Listar propriedades e relações dos [objetos vulnerableManagedDevice.](../resources/intune-partnerintegration-vulnerablemanageddevice.md)|
|[Obter vulnerableManagedDevice](../api/intune-partnerintegration-vulnerablemanageddevice-get.md)|[vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md)|Leia propriedades e relações do [objeto vulnerableManagedDevice.](../resources/intune-partnerintegration-vulnerablemanageddevice.md)|
|[Criar vulnerableManagedDevice](../api/intune-partnerintegration-vulnerablemanageddevice-create.md)|[vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md)|Crie um novo [objeto vulnerableManagedDevice.](../resources/intune-partnerintegration-vulnerablemanageddevice.md)|
|[Excluir vulnerableManagedDevice](../api/intune-partnerintegration-vulnerablemanageddevice-delete.md)|Nenhum|Exclui um [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md).|
|[Atualizar vulnerableManagedDevice](../api/intune-partnerintegration-vulnerablemanageddevice-update.md)|[vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md)|Atualize as propriedades de [um objeto vulnerableManagedDevice.](../resources/intune-partnerintegration-vulnerablemanageddevice.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A chave de entidade e a ID do dispositivo AAD.|
|managedDeviceId|Cadeia de Caracteres|A ID do dispositivo gerenciado do Intune.|
|displayName|Cadeia de caracteres|O nome do dispositivo.|
|lastSyncDateTime|DateTimeOffset|A última data de sincronização.|

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



