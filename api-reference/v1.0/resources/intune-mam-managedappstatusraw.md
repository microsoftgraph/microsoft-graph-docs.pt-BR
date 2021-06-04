---
title: tipo de recurso managedAppStatusRaw
description: Representa um relatório de status não digitado sobre configuração e proteção de aplicativos para organizações.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1d29ec2d96d38c6bc1f2fccf5fb5b36e16e1c5be
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752767"
---
# <a name="managedappstatusraw-resource-type"></a>tipo de recurso managedAppStatusRaw

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um relatório de status não digitado sobre configuração e proteção de aplicativos para organizações.


Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedAppStatusRaws](../api/intune-mam-managedappstatusraw-list.md)|Conjunto [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)|Listar propriedades e relações de objetos de [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).|
|[Obter managedAppStatusRaw](../api/intune-mam-managedappstatusraw-get.md)|[managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md)|Ler propriedades e relações do objeto [managedAppStatusRaw](../resources/intune-mam-managedappstatusraw.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|Nome amigável do relatório de status. Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)|
|id|Cadeia de caracteres|Chave da entidade. Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)|
|version|String|Versão da entidade. Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)|
|content|[Json](../resources/intune-mam-json.md)|Conteúdo do relatório de status.|

## <a name="relationships"></a>Relações
Nenhuma

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




