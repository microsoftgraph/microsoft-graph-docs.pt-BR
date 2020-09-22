---
title: tipo de recurso appLogCollectionRequest
description: Entidade AppLogCollectionRequest.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2fac40719f01144917ad80bc272037c1f81c6b78
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060850"
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
|id|Cadeia de caracteres|O identificador exclusivo. É userId_DeviceId_AppId ID.|
|status|[appLogUploadState](../resources/intune-devices-apploguploadstate.md)|Status de carregamento de logs. Os valores possíveis são: `pending`, `completed`, `failed`.|
|errorMessage|Cadeia de caracteres|Mensagem de erro se qualquer um durante o processo de carregamento|
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






