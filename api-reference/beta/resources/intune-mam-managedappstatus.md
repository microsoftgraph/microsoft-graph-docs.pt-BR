---
title: Tipo de recurso managedAppStatus
description: Representa o status de proteção e configuração do aplicativo para a organização.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e3a43214f2c9157de1ebf690eb9d43504e5224d7
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49266785"
---
# <a name="managedappstatus-resource-type"></a>Tipo de recurso managedAppStatus

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa o status de proteção e configuração do aplicativo para a organização.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedAppStatuses](../api/intune-mam-managedappstatus-list.md)|Conjunto [managedAppStatus](../resources/intune-mam-managedappstatus.md)|Listar propriedades e as relações de objetos de [managedAppStatus](../resources/intune-mam-managedappstatus.md).|
|[Obter managedAppStatus](../api/intune-mam-managedappstatus-get.md)|[managedAppStatus](../resources/intune-mam-managedappstatus.md)|Ler propriedades e relações de objetos de [managedAppStatus](../resources/intune-mam-managedappstatus.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|Nome amigável do relatório de status.|
|id|String|Chave da entidade.|
|versão|String|Versão da entidade.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatus",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String"
}
```




