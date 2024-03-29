---
title: tipo de recurso payloadCompatibleAssignmentFilter
description: Uma classe que contém as propriedades usadas para Filtro de Atribuição Compatível com Carga.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5d21f632254b77b69ecdc96179d3a7a69418c180
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59074889"
---
# <a name="payloadcompatibleassignmentfilter-resource-type"></a>tipo de recurso payloadCompatibleAssignmentFilter

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe que contém as propriedades usadas para Filtro de Atribuição Compatível com Carga.


Herda de [deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar payloadCompatibleAssignmentFilters](../api/intune-policyset-payloadcompatibleassignmentfilter-list.md)|[coleção payloadCompatibleAssignmentFilter](../resources/intune-policyset-payloadcompatibleassignmentfilter.md)|Listar propriedades e relações dos objetos [payloadCompatibleAssignmentFilter.](../resources/intune-policyset-payloadcompatibleassignmentfilter.md)|
|[Obter payloadCompatibleAssignmentFilter](../api/intune-policyset-payloadcompatibleassignmentfilter-get.md)|[payloadCompatibleAssignmentFilter](../resources/intune-policyset-payloadcompatibleassignmentfilter.md)|Leia propriedades e relações do [objeto payloadCompatibleAssignmentFilter.](../resources/intune-policyset-payloadcompatibleassignmentfilter.md)|
|[Criar payloadCompatibleAssignmentFilter](../api/intune-policyset-payloadcompatibleassignmentfilter-create.md)|[payloadCompatibleAssignmentFilter](../resources/intune-policyset-payloadcompatibleassignmentfilter.md)|Crie um novo [objeto payloadCompatibleAssignmentFilter.](../resources/intune-policyset-payloadcompatibleassignmentfilter.md)|
|[Excluir payloadCompatibleAssignmentFilter](../api/intune-policyset-payloadcompatibleassignmentfilter-delete.md)|Nenhum|Exclui um [payloadCompatibleAssignmentFilter](../resources/intune-policyset-payloadcompatibleassignmentfilter.md).|
|[Atualizar payloadCompatibleAssignmentFilter](../api/intune-policyset-payloadcompatibleassignmentfilter-update.md)|[payloadCompatibleAssignmentFilter](../resources/intune-policyset-payloadcompatibleassignmentfilter.md)|Atualize as propriedades de [um objeto payloadCompatibleAssignmentFilter.](../resources/intune-policyset-payloadcompatibleassignmentfilter.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave do Filtro de Atribuição. Herdado [de deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|createdDateTime|DateTimeOffset|Hora de criação do Filtro de Atribuição. Herdado [de deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|lastModifiedDateTime|DateTimeOffset|Última hora modificada do Filtro de Atribuição. Herdado [de deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|displayName|String|DisplayName do Filtro de Atribuição. Herdado [de deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|description|Cadeia de caracteres|Descrição do Filtro de Atribuição. Herdado [de deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|plataforma|[devicePlatformType](../resources/intune-policyset-deviceplatformtype.md)|Tipo de plataforma dos dispositivos nos quais o Filtro de Atribuição será aplicável. Herdado [de deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md). Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|
|rule|Cadeia de caracteres|Definição de regra do Filtro de Atribuição. Herdado [de deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|roleScopeTags|Conjunto de cadeias de caracteres|RoleScopeTags do Filtro de Atribuição. Herdado [de deviceAndAppManagementAssignmentFilter](../resources/intune-policyset-deviceandappmanagementassignmentfilter.md)|
|payloadType|[assignmentFilterPayloadType](../resources/intune-policyset-assignmentfilterpayloadtype.md)|PayloadType do Filtro de Atribuição. Os valores possíveis são: `notSet`, `enrollmentRestrictions`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.payloadCompatibleAssignmentFilter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.payloadCompatibleAssignmentFilter",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "platform": "String",
  "rule": "String",
  "roleScopeTags": [
    "String"
  ],
  "payloadType": "String"
}
```



