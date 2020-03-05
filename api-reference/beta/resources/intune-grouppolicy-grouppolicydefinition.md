---
title: tipo de recurso groupPolicyDefinition
description: A entidade descreve todas as informações sobre uma única diretiva de grupo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 038647f4e40036db89ecf61cdece531662658c46
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528090"
---
# <a name="grouppolicydefinition-resource-type"></a>tipo de recurso groupPolicyDefinition

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade descreve todas as informações sobre uma única diretiva de grupo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter groupPolicyDefinition](../api/intune-grouppolicy-grouppolicydefinition-get.md)|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|Leia as propriedades e as relações do objeto [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) .|
|[Atualizar groupPolicyDefinition](../api/intune-grouppolicy-grouppolicydefinition-update.md)|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|Atualiza as propriedades de um objeto [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|classType|[groupPolicyDefinitionClassType](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|Identifica o tipo de grupo ao qual a política pode ser aplicada. Os valores possíveis são: `user` e `machine`.|
|displayName|Cadeia de caracteres|O nome da política localizada.|
|Texto não criptografado|String|A explicação localizada ou o texto de ajuda associado à política. O valor padrão é vazio.|
|categoryPath|String|O caminho de categoria completo localizado para a política.|
|com suporte|String|Cadeia de caracteres localizada usada para especificar o sistema operacional ou a versão do aplicativo é afetada pela política.|
|PolicyType|[groupPolicyType](../resources/intune-grouppolicy-grouppolicytype.md)|Especifica o tipo de política de grupo. Os valores possíveis são: `admxBacked` e `admxIngested`.|
|id|String|Chave da entidade.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a entidade foi modificada pela última vez.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|DefinitionFile|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|O arquivo de política de grupo associado à definição.|
|apresentações|coleção [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|As apresentações de política de grupo associadas à definição.|

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



