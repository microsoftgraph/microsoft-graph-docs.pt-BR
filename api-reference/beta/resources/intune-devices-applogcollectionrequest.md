---
title: tipo de recurso appLogCollectionRequest
description: Entidade AppLogCollectionRequest.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9c3c3c1f07a6fa0cd5d9ea4ad764e67753f840e9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49267884"
---
# <a name="applogcollectionrequest-resource-type"></a>tipo de recurso appLogCollectionRequest

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade AppLogCollectionRequest.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar appLogCollectionRequests](../api/intune-devices-applogcollectionrequest-list.md)|coleção [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)|Listar Propriedades e relações dos objetos [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) .|
|[Obter appLogCollectionRequest](../api/intune-devices-applogcollectionrequest-get.md)|[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)|Leia as propriedades e as relações do objeto [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) .|
|[Criar appLogCollectionRequest](../api/intune-devices-applogcollectionrequest-create.md)|[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)|Criar um novo objeto [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) .|
|[Excluir appLogCollectionRequest](../api/intune-devices-applogcollectionrequest-delete.md)|Nenhum|Exclui [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md).|
|[Atualizar appLogCollectionRequest](../api/intune-devices-applogcollectionrequest-update.md)|[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)|Atualiza as propriedades de um objeto [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) .|
|[ação createDownloadUrl](../api/intune-devices-applogcollectionrequest-createdownloadurl.md)|[appLogCollectionDownloadDetails](../resources/intune-devices-applogcollectiondownloaddetails.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo. É userId_DeviceId_AppId ID.|
|status|[appLogUploadState](../resources/intune-devices-apploguploadstate.md)|Status de carregamento de logs. Os valores possíveis são: `pending`, `completed`, `failed`.|
|errorMessage|String|Mensagem de erro se qualquer um durante o processo de carregamento|
|customLogFolders|Coleção de cadeias de caracteres|Lista de pastas de log. |
|completedDateTime|DateTimeOffset|Hora em que a solicitação de log de carregamento alcançou um estado de terminal|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appLogCollectionRequest"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appLogCollectionRequest",
  "id": "String (identifier)",
  "status": "String",
  "errorMessage": "String",
  "customLogFolders": [
    "String"
  ],
  "completedDateTime": "String (timestamp)"
}
```




