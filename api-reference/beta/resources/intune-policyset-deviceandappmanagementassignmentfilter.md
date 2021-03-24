---
title: Tipo de recurso deviceAndAppManagementAssignmentFilter
description: Uma classe que contém as propriedades usadas para Filtro de Atribuição.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c8b0811bd8ab91aca4ad71c72cc9691193172e6c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51130634"
---
# <a name="deviceandappmanagementassignmentfilter-resource-type"></a>Tipo de recurso deviceAndAppManagementAssignmentFilter

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe que contém as propriedades usadas para Filtro de Atribuição.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceAndAppManagementAssignmentFilters](../api/intune-policyset-deviceandappmanagementassignmentfilter-list.md)|[Coleção deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|Listar propriedades e relações dos [objetos deviceAndAppManagementAssignmentFilter.](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|[Obter deviceAndAppManagementAssignmentFilter](../api/intune-policyset-deviceandappmanagementassignmentfilter-get.md)|[deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|Leia propriedades e relações do [objeto deviceAndAppManagementAssignmentFilter.](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|[Criar deviceAndAppManagementAssignmentFilter](../api/intune-policyset-deviceandappmanagementassignmentfilter-create.md)|[deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|Crie um novo [objeto deviceAndAppManagementAssignmentFilter.](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|[Excluir deviceAndAppManagementAssignmentFilter](../api/intune-policyset-deviceandappmanagementassignmentfilter-delete.md)|Nenhum|Exclui um [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md).|
|[Atualizar deviceAndAppManagementAssignmentFilter](../api/intune-policyset-deviceandappmanagementassignmentfilter-update.md)|[deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|Atualize as propriedades de [um objeto deviceAndAppManagementAssignmentFilter.](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|[Ação validateFilter](../api/intune-policyset-deviceandappmanagementassignmentfilter-validatefilter.md)|[assignmentFilterValidationResult](../resources/intune-policyset-assignmentfiltervalidationresult.md)|Ainda não documentado|
|[habilitar ação](../api/intune-policyset-deviceandappmanagementassignmentfilter-enable.md)|Nenhuma|Ainda não documentado|
|[função getState](../api/intune-policyset-deviceandappmanagementassignmentfilter-getstate.md)|[assignmentFilterState](../resources/intune-policyset-assignmentfilterstate.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave do Filtro de Atribuição.|
|createdDateTime|DateTimeOffset|Hora de criação do Filtro de Atribuição.|
|lastModifiedDateTime|DateTimeOffset|Última hora modificada do Filtro de Atribuição.|
|displayName|Cadeia de caracteres|DisplayName do Filtro de Atribuição.|
|descrição|Cadeia de caracteres|Descrição do Filtro de Atribuição.|
|plataforma|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)|Tipo de plataforma dos dispositivos nos quais o Filtro de Atribuição será aplicável. Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|
|rule|Cadeia de caracteres|Definição de regra do Filtro de Atribuição.|
|roleScopeTags|Coleção de cadeias de caracteres|RoleScopeTags do Filtro de Atribuição.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentFilter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementAssignmentFilter",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "platform": "String",
  "rule": "String",
  "roleScopeTags": [
    "String"
  ]
}
```




