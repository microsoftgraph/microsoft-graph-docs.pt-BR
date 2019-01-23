---
title: tipo de recurso de groupPolicyDefinition
description: A entidade descreve todas as informações sobre uma diretiva de grupo único.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 502312f7a39dd5dc93fd8e39203f56d47a9ebf27
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429195"
---
# <a name="grouppolicydefinition-resource-type"></a>tipo de recurso de groupPolicyDefinition

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

A entidade descreve todas as informações sobre uma diretiva de grupo único.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter groupPolicyDefinition](../api/intune-grouppolicy-grouppolicydefinition-get.md)|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|Leia as propriedades e os relacionamentos do objeto [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) .|
|[Atualizar groupPolicyDefinition](../api/intune-grouppolicy-grouppolicydefinition-update.md)|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|Atualize as propriedades de um objeto [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|classType|[groupPolicyDefinitionClassType](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|Identifica o tipo dos grupos a que a diretiva pode ser aplicada. Os valores possíveis são: `user`, `machine`, `both`.|
|displayName|String|O nome da política localizado.|
|explainText|String|A explicação ou ajuda texto localizado associado à política. O valor padrão é vazio.|
|categoryPath|String|O caminho de categoria completo localizado para a política.|
|supportedOn|String|A cadeia de caracteres localizada é usada para especificar qual sistema operacional ou a versão do aplicativo é afetada pela diretiva.|
|policyType|[groupPolicyType](../resources/intune-grouppolicy-grouppolicytype.md)|Especifica o tipo de política de grupo. Os valores possíveis são: `admxBacked` e `admxIngested`.|
|id|String|Chave da entidade.|
|lastModifiedDateTime|DateTimeOffset|A data e hora que a entidade foi modificado pela última vez.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|definitionFile|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|O arquivo de diretiva de grupo associado à definição.|
|apresentações|coleção [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|As apresentações de diretiva de grupo associadas à definição.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyDefinition",
  "classType": "String",
  "displayName": "String",
  "explainText": "String",
  "categoryPath": "String",
  "supportedOn": "String",
  "policyType": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




