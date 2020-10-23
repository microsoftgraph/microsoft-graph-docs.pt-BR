---
title: tipo de recurso managementConditionStatement
description: Uma instrução de condição de gerenciamento é um grupo de condições de gerenciamento que Habilita/desabilita as configurações de dispositivo/aplicativo quando todas as condições de gerenciamento contidas são atendidas.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a5bebd514c4a24bd9a19b1a23c5b354c330d2bdf
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48722841"
---
# <a name="managementconditionstatement-resource-type"></a>tipo de recurso managementConditionStatement

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma instrução de condição de gerenciamento é um grupo de condições de gerenciamento que Habilita/desabilita as configurações de dispositivo/aplicativo quando todas as condições de gerenciamento contidas são atendidas.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managementConditionStatements](../api/intune-fencing-managementconditionstatement-list.md)|coleção [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|Listar Propriedades e relações dos objetos [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) .|
|[Obter managementConditionStatement](../api/intune-fencing-managementconditionstatement-get.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|Leia as propriedades e as relações do objeto [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) .|
|[Criar managementConditionStatement](../api/intune-fencing-managementconditionstatement-create.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|Criar um novo objeto [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) .|
|[Excluir managementConditionStatement](../api/intune-fencing-managementconditionstatement-delete.md)|Nenhum|Exclui [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md).|
|[Atualizar managementConditionStatement](../api/intune-fencing-managementconditionstatement-update.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|Atualiza as propriedades de um objeto [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) .|
|[função getManagementConditionStatementExpressionString](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementexpressionstring.md)|[managementConditionExpressionString](../resources/intune-fencing-managementconditionexpressionstring.md)|Ainda não documentado|
|[função getManagementConditionStatementsForPlatform](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementsforplatform.md)|coleção [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo da instrução de condição de gerenciamento. Valor gerado pelo sistema atribuído quando criado.|
|displayName|String|O nome do administrador definido da instrução de condição de gerenciamento.|
|description|String|A descrição definida pelo administrador da instrução de condição de gerenciamento.|
|createdDateTime|DateTimeOffset|A hora em que a instrução de gerenciamento da condição foi criada. Lado do serviço gerado.|
|modifiedDateTime|DateTimeOffset|A hora em que a declaração de condição de gerenciamento foi modificada pela última vez. Atualizado o lado do serviço.|
|expressão|[managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)|A expressão de instrução de condição de gerenciamento usada para avaliar se uma instrução de condição de gerenciamento foi ativada/desativada.|
|eTag|String|ETag da instrução de condição de gerenciamento. Atualizado o lado do serviço.|
|applicablePlatforms|coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)|As plataformas aplicáveis para essa instrução de condição de gerenciamento.
Isso é calculado a partir da aparência das condições de gerenciamento associadas à instrução de condição de gerenciamento e à localização da interseção de plataformas aplicáveis.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|managementConditions|coleção [managementCondition](../resources/intune-fencing-managementcondition.md)|As condições de gerenciamento associadas à instrução de condição de gerenciamento.|

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





