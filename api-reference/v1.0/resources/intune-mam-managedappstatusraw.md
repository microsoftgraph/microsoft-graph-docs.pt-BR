---
title: tipo de recurso managedAppStatusRaw
description: Representa um relatório de status não digitado sobre configuração e proteção de aplicativos para organizações.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b21c15784409d9d7c373c954faecbc23426041b1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037874"
---
# <a name="managedappstatusraw-resource-type"></a>tipo de recurso managedAppStatusRaw

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um relatório de status não digitado sobre configuração e proteção de aplicativos para organizações.


Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedAppStatusRaws](../api/intune-mam-managedappstatusraw-list.md)|Conjunto [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)|Listar propriedades e relações de objetos de [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).|
|[Obter managedAppStatusRaw](../api/intune-mam-managedappstatusraw-get.md)|[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)|Ler propriedades e relações do objeto [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|Nome amigável do relatório de status. Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)|
|id|String|Chave da entidade. Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)|
|version|String|Versão da entidade. Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)|
|content|[Json](../resources/intune-mam-json.md)|Conteúdo do relatório de status.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppStatusRaw"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppStatusRaw",
  "displayName": "String",
  "id": "String (identifier)",
  "version": "String",
  "content": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```



