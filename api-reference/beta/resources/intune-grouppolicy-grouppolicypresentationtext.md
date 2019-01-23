---
title: tipo de recurso de groupPolicyPresentationText
description: Representa um elemento de texto ADMX.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b380bc5a52423279a0a724b8b6b0e9c7cf638cbc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429266"
---
# <a name="grouppolicypresentationtext-resource-type"></a>tipo de recurso de groupPolicyPresentationText

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Representa um elemento de texto ADMX.


Herda de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista groupPolicyPresentationTexts](../api/intune-grouppolicy-grouppolicypresentationtext-list.md)|coleção [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md)|Lista as propriedades e os relacionamentos dos objetos [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) .|
|[Obter groupPolicyPresentationText](../api/intune-grouppolicy-grouppolicypresentationtext-get.md)|[groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md)|Leia as propriedades e os relacionamentos do objeto [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) .|
|[Criar groupPolicyPresentationText](../api/intune-grouppolicy-grouppolicypresentationtext-create.md)|[groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md)|Crie um novo objeto de [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) .|
|[Excluir groupPolicyPresentationText](../api/intune-grouppolicy-grouppolicypresentationtext-delete.md)|Nenhum|Exclui um [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md).|
|[Atualizar groupPolicyPresentationText](../api/intune-grouppolicy-grouppolicypresentationtext-update.md)|[groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md)|Atualize as propriedades de um objeto [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|rótulo|String|Rótulo de texto localizado para qualquer entidade de apresentação. O valor padrão é vazio. Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|String|Chave da entidade. Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|A data e hora que a entidade foi modificado pela última vez. Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|definição|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|A definição de política de grupo associada à apresentação. Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationText"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationText",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




