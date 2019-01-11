---
title: tipo de recurso managedAppStatusRaw
description: Representa um relatório de status não digitado sobre configuração e proteção de aplicativos para organizações.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 975f43d064718b8457b40be707a54a0ea0eb69f7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884011"
---
# <a name="managedappstatusraw-resource-type"></a>tipo de recurso managedAppStatusRaw

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

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
|id|Cadeia de caracteres|Chave da entidade. Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)|
|version|Cadeia de caracteres|Versão da entidade. Herda de [managedAppStatus](../resources/intune-mam-managedappstatus.md)|
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





