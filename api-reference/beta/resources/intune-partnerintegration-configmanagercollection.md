---
title: Tipo de recurso configManagerCollection
description: Uma coleção definida configManager de dispositivos ou usuários.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d7c4300dc1cedbc316e6e8cfa5c0efebd1e383f8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59033459"
---
# <a name="configmanagercollection-resource-type"></a>Tipo de recurso configManagerCollection

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma coleção definida configManager de dispositivos ou usuários.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar configManagerCollections](../api/intune-partnerintegration-configmanagercollection-list.md)|[Coleção configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md)|Listar propriedades e relações dos [objetos configManagerCollection.](../resources/intune-partnerintegration-configmanagercollection.md)|
|[Obter configManagerCollection](../api/intune-partnerintegration-configmanagercollection-get.md)|[configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md)|Ler propriedades e relações do [objeto configManagerCollection.](../resources/intune-partnerintegration-configmanagercollection.md)|
|[Criar configManagerCollection](../api/intune-partnerintegration-configmanagercollection-create.md)|[configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md)|Crie um novo [objeto configManagerCollection.](../resources/intune-partnerintegration-configmanagercollection.md)|
|[Excluir configManagerCollection](../api/intune-partnerintegration-configmanagercollection-delete.md)|Nenhum|Exclui um [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md).|
|[Atualizar configManagerCollection](../api/intune-partnerintegration-configmanagercollection-update.md)|[configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md)|Atualize as propriedades de [um objeto configManagerCollection.](../resources/intune-partnerintegration-configmanagercollection.md)|
|[função getPolicySummary](../api/intune-partnerintegration-configmanagercollection-getpolicysummary.md)|[configManagerPolicySummary](../resources/intune-partnerintegration-configmanagerpolicysummary.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A chave da Coleção ConfigManager.|
|displayName|Cadeia de caracteres|The DisplayName.|
|collectionIdentifier|String|O identificador de coleção no SCCM.|
|hierarchyName|Cadeia de Caracteres|O HierarchyName.|
|hierarchyIdentifier|Cadeia de caracteres|O Identificador de Hierarquia.|
|createdDateTime|DateTimeOffset|A data criada.|
|lastModifiedDateTime|DateTimeOffset|A última data modificada.|

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



