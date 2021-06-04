---
title: Tipo de recurso managedAppPolicy
description: O recurso ManagedAppPolicy representa um tipo de base para políticas específicas de plataformas.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 61fedfab47ee44d187d2de81c0699885c4af06f4
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752774"
---
# <a name="managedapppolicy-resource-type"></a>Tipo de recurso managedAppPolicy

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O recurso ManagedAppPolicy representa um tipo de base para políticas específicas de plataformas.

## <a name="methods"></a>Methods
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
|versão|String|Versão da entidade.|

## <a name="relationships"></a>Relações
Nenhuma

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




