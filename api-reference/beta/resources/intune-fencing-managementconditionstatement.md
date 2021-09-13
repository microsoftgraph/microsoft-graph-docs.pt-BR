---
title: Tipo de recurso managementConditionStatement
description: Uma instrução de condição de gerenciamento é um grupo de condições de gerenciamento que habilita/desabilita configurações de dispositivo/aplicativo quando todas as condições de gerenciamento contidas são atendidas.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6a4223de89f7c7dfaf79e5f0bd2494d354654506
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59063962"
---
# <a name="managementconditionstatement-resource-type"></a>Tipo de recurso managementConditionStatement

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma instrução de condição de gerenciamento é um grupo de condições de gerenciamento que habilita/desabilita configurações de dispositivo/aplicativo quando todas as condições de gerenciamento contidas são atendidas.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Gerenciamento de listasConditionStatements](../api/intune-fencing-managementconditionstatement-list.md)|[coleção managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|Listar propriedades e relações dos objetos [managementConditionStatement.](../resources/intune-fencing-managementconditionstatement.md)|
|[Obter managementConditionStatement](../api/intune-fencing-managementconditionstatement-get.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|Leia propriedades e relações do [objeto managementConditionStatement.](../resources/intune-fencing-managementconditionstatement.md)|
|[Criar managementConditionStatement](../api/intune-fencing-managementconditionstatement-create.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|Crie um novo [objeto managementConditionStatement.](../resources/intune-fencing-managementconditionstatement.md)|
|[Excluir managementConditionStatement](../api/intune-fencing-managementconditionstatement-delete.md)|Nenhum|Exclui um [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md).|
|[Atualizar managementConditionStatement](../api/intune-fencing-managementconditionstatement-update.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|Atualize as propriedades de [um objeto managementConditionStatement.](../resources/intune-fencing-managementconditionstatement.md)|
|[função getManagementConditionStatementExpressionString](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementexpressionstring.md)|[managementConditionExpressionString](../resources/intune-fencing-managementconditionexpressionstring.md)|Ainda não documentado|
|[função getManagementConditionStatementsForPlatform](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementsforplatform.md)|[coleção managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo para a instrução de condição de gerenciamento. Valor gerado pelo sistema atribuído quando criado.|
|displayName|String|O nome definido pelo administrador da instrução de condição de gerenciamento.|
|description|Cadeia de caracteres|A descrição definida pelo administrador da instrução de condição de gerenciamento.|
|createdDateTime|DateTimeOffset|A hora em que a instrução de condição de gerenciamento foi criada. Lado de serviço gerado.|
|modifiedDateTime|DateTimeOffset|A hora em que a instrução de condição de gerenciamento foi modificada pela última vez. Lado do serviço atualizado.|
|expressão|[managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)|A expressão de instrução de condição de gerenciamento usada para avaliar se uma instrução de condição de gerenciamento foi ativada/desativada.|
|eTag|String|ETag da instrução de condição de gerenciamento. Lado do serviço atualizado.|
|applicablePlatforms|[Coleção devicePlatformType](../resources/intune-fencing-deviceplatformtype.md)|As plataformas aplicáveis para essa instrução de condição de gerenciamento.
Isso é calculado analisando as condições de gerenciamento associadas à instrução de condição de gerenciamento e encontrando a interseção das plataformas aplicáveis.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|managementConditions|[coleção managementCondition](../resources/intune-fencing-managementcondition.md)|As condições de gerenciamento associadas à instrução de condição de gerenciamento.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managementConditionStatement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpressionString",
    "value": "String"
  },
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ]
}
```



