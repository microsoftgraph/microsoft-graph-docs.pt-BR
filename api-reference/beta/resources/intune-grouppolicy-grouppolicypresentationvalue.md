---
title: tipo de recurso de groupPolicyPresentationValue
description: A entidade de valor de base de apresentação que armazena o valor de uma apresentação de diretiva de grupo único.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ec299eccc29ddcb39ece0d1f6c0e063a02192909
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29428963"
---
# <a name="grouppolicypresentationvalue-resource-type"></a>tipo de recurso de groupPolicyPresentationValue

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

A entidade de valor de base de apresentação que armazena o valor de uma apresentação de diretiva de grupo único.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista groupPolicyPresentationValues](../api/intune-grouppolicy-grouppolicypresentationvalue-list.md)|coleção [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|Lista as propriedades e os relacionamentos dos objetos [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) .|
|[Obter groupPolicyPresentationValue](../api/intune-grouppolicy-grouppolicypresentationvalue-get.md)|[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|Leia as propriedades e os relacionamentos do objeto [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) .|
|[Criar groupPolicyPresentationValue](../api/intune-grouppolicy-grouppolicypresentationvalue-create.md)|[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|Crie um novo objeto de [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) .|
|[Excluir groupPolicyPresentationValue](../api/intune-grouppolicy-grouppolicypresentationvalue-delete.md)|Nenhum|Exclui um [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md).|
|[Atualizar groupPolicyPresentationValue](../api/intune-grouppolicy-grouppolicypresentationvalue-update.md)|[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|Atualize as propriedades de um objeto [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|A data e hora que da última modificação do objeto.|
|createdDateTime|DateTimeOffset|A data e hora que o objeto foi criado.|
|id|String|Chave da entidade.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|definitionValue|[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|O valor de definição de política do grupo associado com o valor de apresentação.|
|apresentação|[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|A apresentação de diretiva de grupo associada com o valor de apresentação.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)"
}
```




