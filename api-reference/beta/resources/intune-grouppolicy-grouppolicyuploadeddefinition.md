---
title: Tipo de recurso groupPolicyUploadedDefinition
description: A entidade descreve todas as informações sobre uma única política de grupo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6028f766a49317eeef41aaea5f5f84ddd5390412
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58266923"
---
# <a name="grouppolicyuploadeddefinition-resource-type"></a>Tipo de recurso groupPolicyUploadedDefinition

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade descreve todas as informações sobre uma única política de grupo.


Herda de [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar groupPolicyUploadedDefinitions](../api/intune-grouppolicy-grouppolicyuploadeddefinition-list.md)|[coleção groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md)|Listar propriedades e relações dos [objetos groupPolicyUploadedDefinition.](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md)|
|[Obter groupPolicyUploadedDefinition](../api/intune-grouppolicy-grouppolicyuploadeddefinition-get.md)|[groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md)|Leia propriedades e relações do [objeto groupPolicyUploadedDefinition.](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md)|
|[Criar groupPolicyUploadedDefinition](../api/intune-grouppolicy-grouppolicyuploadeddefinition-create.md)|[groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md)|Crie um novo [objeto groupPolicyUploadedDefinition.](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md)|
|[Excluir groupPolicyUploadedDefinition](../api/intune-grouppolicy-grouppolicyuploadeddefinition-delete.md)|Nenhum|Exclui um [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md).|
|[Atualizar groupPolicyUploadedDefinition](../api/intune-grouppolicy-grouppolicyuploadeddefinition-update.md)|[groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md)|Atualize as propriedades de [um objeto groupPolicyUploadedDefinition.](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|classType|[groupPolicyDefinitionClassType](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|Identifica o tipo de grupos aos qual a política pode ser aplicada. Herdado [de groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md). Os valores possíveis são: `user` e `machine`.|
|displayName|Cadeia de caracteres|O nome da política localizada. Herdado [de groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|explainText|Cadeia de caracteres|A explicação localizada ou o texto de ajuda associado à política. O valor padrão é vazio. Herdado [de groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|categoryPath|Cadeia de caracteres|O caminho de categoria completa localizado para a política. Herdado [de groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|supportedOn|Cadeia de caracteres|Cadeia de caracteres localizada usada para especificar qual versão do sistema operacional ou aplicativo é afetada pela política. Herdado [de groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|policyType|[groupPolicyType](../resources/intune-grouppolicy-grouppolicytype.md)|Especifica o tipo de política de grupo. Herdado [de groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md). Os valores possíveis são: `admxBacked` e `admxIngested`.|
|hasRelatedDefinitions|Boolean|Significa se há ou não definições relacionadas a essa definição Herdadas de [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|groupPolicyCategoryId|Guid|A id de categoria da categoria pai Herdada de [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|versão|String|Definindo a versão de definição Herdada [de groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|id|Cadeia de caracteres|Chave da entidade. Herdado [de groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a entidade foi modificada pela última vez. Herdado [de groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|definitionFile|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|O arquivo de política de grupo associado à definição. Herdado [de groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|category|[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|A categoria de política de grupo associada à definição. Herdado [de groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|apresentações|[coleção groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|As apresentações de política de grupo associadas à definição. Herdado [de groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|previousVersionDefinition|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|Definição da versão anterior dessa definição Herdada de [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|nextVersionDefinition|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|Definição da próxima versão dessa definição Herdada de [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyUploadedDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinition",
  "classType": "String",
  "displayName": "String",
  "explainText": "String",
  "categoryPath": "String",
  "supportedOn": "String",
  "policyType": "String",
  "hasRelatedDefinitions": true,
  "groupPolicyCategoryId": "Guid",
  "version": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




