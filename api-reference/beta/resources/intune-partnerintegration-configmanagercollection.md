---
title: tipo de recurso configManagerCollection
description: Um Configmanager definido como um conjunto de dispositivos ou usuários.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3bc7d7d371a0bbc07b29835c5ed2a4b23078cf04
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301611"
---
# <a name="configmanagercollection-resource-type"></a>tipo de recurso configManagerCollection

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Um Configmanager definido como um conjunto de dispositivos ou usuários.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar configManagerCollections](../api/intune-partnerintegration-configmanagercollection-list.md)|coleção [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md)|Listar Propriedades e relações dos objetos [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) .|
|[Obter configManagerCollection](../api/intune-partnerintegration-configmanagercollection-get.md)|[configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md)|Leia as propriedades e as relações do objeto [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) .|
|[Criar configManagerCollection](../api/intune-partnerintegration-configmanagercollection-create.md)|[configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md)|Criar um novo objeto [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) .|
|[Excluir configManagerCollection](../api/intune-partnerintegration-configmanagercollection-delete.md)|Nenhum|Exclui [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md).|
|[Atualizar configManagerCollection](../api/intune-partnerintegration-configmanagercollection-update.md)|[configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md)|Atualiza as propriedades de um objeto [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) .|
|[função getPolicySummary](../api/intune-partnerintegration-configmanagercollection-getpolicysummary.md)|[configManagerPolicySummary](../resources/intune-partnerintegration-configmanagerpolicysummary.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A chave da coleção Configmanager.|
|displayName|String|O DisplayName.|
|collectionIdentifier|String|O identificador de coleção no SCCM.|
|HierarchyName|String|O HierarchyName.|
|hierarchyIdentifier|String|O identificador de hierarquia.|
|createdDateTime|DateTimeOffset|A data de criação.|
|lastModifiedDateTime|DateTimeOffset|A data da última modificação.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.configManagerCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configManagerCollection",
  "id": "String (identifier)",
  "displayName": "String",
  "collectionIdentifier": "String",
  "hierarchyName": "String",
  "hierarchyIdentifier": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




