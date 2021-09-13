---
title: Tipo de recurso appLogCollectionRequest
description: Entidade AppLogCollectionRequest.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e2cd37ecd109720bf5a564c64d480037a9bd72fc
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59086306"
---
# <a name="applogcollectionrequest-resource-type"></a>Tipo de recurso appLogCollectionRequest

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade AppLogCollectionRequest.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar appLogCollectionRequests](../api/intune-devices-applogcollectionrequest-list.md)|[Coleção appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)|Listar propriedades e relações dos [objetos appLogCollectionRequest.](../resources/intune-devices-applogcollectionrequest.md)|
|[Obter appLogCollectionRequest](../api/intune-devices-applogcollectionrequest-get.md)|[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)|Leia propriedades e relações do [objeto appLogCollectionRequest.](../resources/intune-devices-applogcollectionrequest.md)|
|[Criar appLogCollectionRequest](../api/intune-devices-applogcollectionrequest-create.md)|[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)|Crie um novo [objeto appLogCollectionRequest.](../resources/intune-devices-applogcollectionrequest.md)|
|[Excluir appLogCollectionRequest](../api/intune-devices-applogcollectionrequest-delete.md)|Nenhum|Exclui um [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md).|
|[Atualizar appLogCollectionRequest](../api/intune-devices-applogcollectionrequest-update.md)|[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)|Atualize as propriedades de um [objeto appLogCollectionRequest.](../resources/intune-devices-applogcollectionrequest.md)|
|[ação createDownloadUrl](../api/intune-devices-applogcollectionrequest-createdownloadurl.md)|[appLogCollectionDownloadDetails](../resources/intune-devices-applogcollectiondownloaddetails.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O Identificador exclusivo. Esta é userId_DeviceId_AppId id.|
|status|[appLogUploadState](../resources/intune-devices-apploguploadstate.md)|Status do carregamento de log. Os valores possíveis são: `pending`, `completed`, `failed`.|
|errorMessage|Cadeia de Caracteres|Mensagem de erro se alguma durante o processo de carregamento|
|customLogFolders|Conjunto de cadeias de caracteres|Lista de pastas de log. |
|completedDateTime|DateTimeOffset|Hora em que a solicitação de log de carregamento atingiu um estado de terminal|

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



