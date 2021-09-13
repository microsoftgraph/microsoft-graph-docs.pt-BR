---
title: Tipo de recurso groupPolicyCategory
description: A entidade de categoria armazena a categoria de uma definição de política de grupo
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bd728c056576e31b37a4c105c62186f97e789fa1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59080958"
---
# <a name="grouppolicycategory-resource-type"></a>Tipo de recurso groupPolicyCategory

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de categoria armazena a categoria de uma definição de política de grupo

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter groupPolicyCategory](../api/intune-grouppolicy-grouppolicycategory-get.md)|[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|Ler propriedades e relações do [objeto groupPolicyCategory.](../resources/intune-grouppolicy-grouppolicycategory.md)|
|[Atualizar groupPolicyCategory](../api/intune-grouppolicy-grouppolicycategory-update.md)|[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|Atualize as propriedades de [um objeto groupPolicyCategory.](../resources/intune-grouppolicy-grouppolicycategory.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|A id de cadeia de caracteres do nome de exibição da categoria|
|isRoot|Boolean|Define se a categoria é uma categoria raiz|
|id|String|Chave da entidade.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a entidade foi modificada pela última vez.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|primário|[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|A categoria pai|
|children|[coleção groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|As categorias de filhos|
|definições|[coleção groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|Os filhos de GroupPolicyDefinition imediatos da categoria|
|definitionFile|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|A id do arquivo de definição de onde a categoria veio|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyCategory",
  "displayName": "String",
  "isRoot": true,
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```



