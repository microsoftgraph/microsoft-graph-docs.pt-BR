---
title: Tipo de recurso tenantAttachRBAC
description: Entidade singleton que atua como um contêiner para a funcionalidade de habilitação de anexação de locatário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: af582f15444821fba9e36cf23ef1f2c4075ad57c
ms.sourcegitcommit: 0076eb6abb89be3dca3575631924a74a5202be30
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2022
ms.locfileid: "64631064"
---
# <a name="tenantattachrbac-resource-type"></a>Tipo de recurso tenantAttachRBAC

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade singleton que atua como um contêiner para a funcionalidade de habilitação de anexação de locatário.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter tenantAttachRBAC](../api/intune-devices-tenantattachrbac-get.md)|[tenantAttachRBAC](../resources/intune-devices-tenantattachrbac.md)|Leia propriedades e relações do [objeto tenantAttachRBAC](../resources/intune-devices-tenantattachrbac.md) .|
|[Atualizar tenantAttachRBAC](../api/intune-devices-tenantattachrbac-update.md)|[tenantAttachRBAC](../resources/intune-devices-tenantattachrbac.md)|Atualize as propriedades de um [objeto tenantAttachRBAC](../resources/intune-devices-tenantattachrbac.md) .|
|[habilitar ação](../api/intune-devices-tenantattachrbac-enable.md)|Nenhuma|Ainda não documentado|
|[função getState](../api/intune-devices-tenantattachrbac-getstate.md)|[tenantAttachRBACState](../resources/intune-devices-tenantattachrbacstate.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo dessa entidade|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.tenantAttachRBAC"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.tenantAttachRBAC",
  "id": "String (identifier)"
}
```




