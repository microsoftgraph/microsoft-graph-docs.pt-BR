---
title: tipo de recurso groupPolicyPresentationText
description: Representa um elemento de texto do ADMX.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 962dafac2a5e60b5ed72d8c270d888f49e34e35a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941062"
---
# <a name="grouppolicypresentationtext-resource-type"></a>tipo de recurso groupPolicyPresentationText

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um elemento de texto do ADMX.


Herda de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar groupPolicyPresentationTexts](../api/intune-grouppolicy-grouppolicypresentationtext-list.md)|coleção [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md)|Listar Propriedades e relações dos objetos [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) .|
|[Obter groupPolicyPresentationText](../api/intune-grouppolicy-grouppolicypresentationtext-get.md)|[groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md)|Leia as propriedades e as relações do objeto [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) .|
|[Criar groupPolicyPresentationText](../api/intune-grouppolicy-grouppolicypresentationtext-create.md)|[groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md)|Criar um novo objeto [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) .|
|[Excluir groupPolicyPresentationText](../api/intune-grouppolicy-grouppolicypresentationtext-delete.md)|Nenhum|Exclui [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md).|
|[Atualizar groupPolicyPresentationText](../api/intune-grouppolicy-grouppolicypresentationtext-update.md)|[groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md)|Atualiza as propriedades de um objeto [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|rótulo|Cadeia de caracteres|Rótulo de texto localizado para qualquer entidade de apresentação. O valor padrão é vazio. Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|Cadeia de caracteres|Chave da entidade. Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a entidade foi modificada pela última vez. Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|definir|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|A definição de política de grupo associada à apresentação. Herdado de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|

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




