---
title: Tipo de recurso managedAppPolicy
description: O recurso ManagedAppPolicy representa um tipo de base para políticas específicas de plataformas.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5766e3a467a157bac0d876fd0178dc3ba1cb94e2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888078"
---
# <a name="managedapppolicy-resource-type"></a>Tipo de recurso managedAppPolicy

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

O recurso ManagedAppPolicy representa um tipo de base para políticas específicas de plataformas.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedAppPolicies](../api/intune-mam-managedapppolicy-list.md)|Conjunto [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|Listar propriedades e relações de objetos de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|[Obter managedAppPolicy](../api/intune-mam-managedapppolicy-get.md)|[managedAppPolicy](../resources/intune-mam-managedapppolicy.md)|Ler propriedades e relações de objetos de [managedAppPolicy](../resources/intune-mam-managedapppolicy.md).|
|[Ação targetApps](../api/intune-mam-managedapppolicy-targetapps.md)|Nenhum|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|Nome de exibição da política.|
|descrição|Cadeia de caracteres|Descrição da política.|
|createdDateTime|DateTimeOffset|A data e a hora da criação da política.|
|lastModifiedDateTime|DateTimeOffset|Última hora em que a política foi modificada.|
|id|Cadeia de caracteres|Chave da entidade.|
|version|Cadeia de caracteres|Versão da entidade.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicy",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String"
}
```



