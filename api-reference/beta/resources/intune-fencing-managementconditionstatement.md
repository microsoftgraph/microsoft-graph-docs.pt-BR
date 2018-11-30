---
title: tipo de recurso de managementConditionStatement
description: Uma instrução de condição de gerenciamento é um grupo de condições de gerenciamento que habilitar/desabilitar configurações de dispositivo/aplicativo quando todas as condições de gerenciamento contidos forem atendidas.
ms.openlocfilehash: 98b76ce96550d894f8b32f6f6174d5c565e322ae
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037508"
---
# <a name="managementconditionstatement-resource-type"></a>tipo de recurso de managementConditionStatement

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Uma instrução de condição de gerenciamento é um grupo de condições de gerenciamento que habilitar/desabilitar configurações de dispositivo/aplicativo quando todas as condições de gerenciamento contidos forem atendidas.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista managementConditionStatements](../api/intune-fencing-managementconditionstatement-list.md)|coleção [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|Lista as propriedades e os relacionamentos dos objetos [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) .|
|[Obter managementConditionStatement](../api/intune-fencing-managementconditionstatement-get.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|Leia as propriedades e os relacionamentos do objeto [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) .|
|[Criar managementConditionStatement](../api/intune-fencing-managementconditionstatement-create.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|Crie um novo objeto de [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) .|
|[Excluir managementConditionStatement](../api/intune-fencing-managementconditionstatement-delete.md)|Nenhum|Exclui um [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md).|
|[Atualizar managementConditionStatement](../api/intune-fencing-managementconditionstatement-update.md)|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|Atualize as propriedades de um objeto [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) .|
|[função getManagementConditionStatementExpressionString](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementexpressionstring.md)|[managementConditionExpressionString](../resources/intune-fencing-managementconditionexpressionstring.md)|Ainda não documentado|
|[função getManagementConditionStatementsForPlatform](../api/intune-fencing-managementconditionstatement-getmanagementconditionstatementsforplatform.md)|coleção [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo para a declaração de condição de gerenciamento. Valor atribuído quando criado gerado pelo sistema.|
|displayName|String|O nome definido admin da declaração de condição de gerenciamento.|
|description|String|O administrador definidos descrição da declaração de condição de gerenciamento.|
|createdDateTime|DateTimeOffset|A hora em que a declaração de condição de gerenciamento foi criada. Lado de serviço gerado.|
|modifiedDateTime|DateTimeOffset|A hora que da última modificação a declaração de condição de gerenciamento. Lado de serviços atualizado.|
|expressão|[managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)|A expressão da instrução gerenciamento condição usada para avaliar se um gerenciamento de condição instrução foi ativado/desativado.|
|eTag|String|ETag da declaração de condição de gerenciamento. Lado de serviços atualizado.|
|applicablePlatforms|coleção [devicePlatformType](../resources/intune-shared-deviceplatformtype.md)|As plataformas aplicáveis para esta declaração de condição de gerenciamento.
Isso é calculado a partir procurando as condições de gerenciamento associadas ao gerenciamento de condição de instrução e encontrar a interseção de plataformas aplicáveis.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|managementConditions|coleção [managementCondition](../resources/intune-fencing-managementcondition.md)|As condições de gerenciamento associadas a declaração de condição de gerenciamento.|

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
    "@odata.type": "microsoft.graph.managementConditionExpression"
  },
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ]
}
```





