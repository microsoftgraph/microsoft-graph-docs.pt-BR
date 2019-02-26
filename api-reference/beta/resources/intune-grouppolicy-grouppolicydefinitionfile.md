---
title: tipo de recurso groupPolicyDefinitionFile
description: A entidade representa um arquivo XML ADMX (modelo administrativo). O arquivo ADMX contém uma coleção de definições de política de grupo e seus locais por caminho de categoria. O arquivo de definição de política de grupo também contém os idiomas suportados conforme determinado pelos arquivos de idioma do ADML (modelo administrativo) dependente de idioma.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 494a2f8ff80b3a7f8ee9db9fea4d795494c19a92
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161331"
---
# <a name="grouppolicydefinitionfile-resource-type"></a>tipo de recurso groupPolicyDefinitionFile

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade representa um arquivo XML ADMX (modelo administrativo). O arquivo ADMX contém uma coleção de definições de política de grupo e seus locais por caminho de categoria. O arquivo de definição de política de grupo também contém os idiomas suportados conforme determinado pelos arquivos de idioma do ADML (modelo administrativo) dependente de idioma.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter groupPolicyDefinitionFile](../api/intune-grouppolicy-grouppolicydefinitionfile-get.md)|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|Leia as propriedades e as relações do objeto [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .|
|[Atualizar groupPolicyDefinitionFile](../api/intune-grouppolicy-grouppolicydefinitionfile-update.md)|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|Atualiza as propriedades de um objeto [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|O nome amigável localizado do arquivo ADMX.|
|descrição|Cadeia de caracteres|A descrição localizada das configurações de política no arquivo ADMX. O valor padrão é vazio.|
|languageCodes|Coleção de cadeias de caracteres|Os códigos de idioma suportados para o arquivo ADMX.|
|targetPrefix|String|Especifica o nome lógico que se refere ao namespace dentro do arquivo ADMX.|
|targetNamespace|String|Especifica o URI usado para identificar o namespace no arquivo ADMX.|
|PolicyType|[groupPolicyType](../resources/intune-grouppolicy-grouppolicytype.md)|Especifica o tipo de política de grupo. Os valores possíveis são: `admxBacked` e `admxIngested`.|
|id|String|Chave da entidade.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a entidade foi modificada pela última vez.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|Definição|coleção [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|As definições de política de grupo associadas ao arquivo.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyDefinitionFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionFile",
  "displayName": "String",
  "description": "String",
  "languageCodes": [
    "String"
  ],
  "targetPrefix": "String",
  "targetNamespace": "String",
  "policyType": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




