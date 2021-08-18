---
title: Tipo de recurso groupPolicyUploadedCategory
description: A entidade de categoria armazena a categoria de uma definição de política de grupo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2b4089b98b4cccb3eb4fda1ea181dbc311e24081247ba3932c46f3ed7c63be57
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54164192"
---
# <a name="grouppolicyuploadedcategory-resource-type"></a>Tipo de recurso groupPolicyUploadedCategory

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de categoria armazena a categoria de uma definição de política de grupo


Herda de [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar groupPolicyUploadedCategories](../api/intune-grouppolicy-grouppolicyuploadedcategory-list.md)|[coleção groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md)|Listar propriedades e relações dos [objetos groupPolicyUploadedCategory.](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md)|
|[Obter groupPolicyUploadedCategory](../api/intune-grouppolicy-grouppolicyuploadedcategory-get.md)|[groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md)|Ler propriedades e relações do [objeto groupPolicyUploadedCategory.](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md)|
|[Criar groupPolicyUploadedCategory](../api/intune-grouppolicy-grouppolicyuploadedcategory-create.md)|[groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md)|Crie um novo [objeto groupPolicyUploadedCategory.](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md)|
|[Excluir groupPolicyUploadedCategory](../api/intune-grouppolicy-grouppolicyuploadedcategory-delete.md)|Nenhum|Exclui um [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md).|
|[Atualizar groupPolicyUploadedCategory](../api/intune-grouppolicy-grouppolicyuploadedcategory-update.md)|[groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md)|Atualize as propriedades de [um objeto groupPolicyUploadedCategory.](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|A id de cadeia de caracteres do nome de exibição da categoria Herdado de [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|
|isRoot|Boolean|Define se a categoria é uma categoria raiz Herdada de [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|
|id|Cadeia de caracteres|Chave da entidade. Herdado [de groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a entidade foi modificada pela última vez. Herdado [de groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|primário|[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|A categoria pai Herdada de [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|
|children|[coleção groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|As categorias filhas Herdadas [de groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|
|definições|[coleção groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|Os filhos de GroupPolicyDefinition imediatos da categoria Herdado de [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|
|definitionFile|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|A id do arquivo de definição que a categoria veio de Inherited from [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyUploadedCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedCategory",
  "displayName": "String",
  "isRoot": true,
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




