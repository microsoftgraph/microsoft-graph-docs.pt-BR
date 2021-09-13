---
title: Tipo de recurso groupPolicyPresentationText
description: Representa um elemento de texto ADMX.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 99a9d3e198151265ae4b740f49c9471c379f5c2c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59085996"
---
# <a name="grouppolicypresentationtext-resource-type"></a>Tipo de recurso groupPolicyPresentationText

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um elemento de texto ADMX.


Herda de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar groupPolicyPresentationTexts](../api/intune-grouppolicy-grouppolicypresentationtext-list.md)|[coleção groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md)|Listar propriedades e relações dos [objetos groupPolicyPresentationText.](../resources/intune-grouppolicy-grouppolicypresentationtext.md)|
|[Obter groupPolicyPresentationText](../api/intune-grouppolicy-grouppolicypresentationtext-get.md)|[groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md)|Leia propriedades e relações do [objeto groupPolicyPresentationText.](../resources/intune-grouppolicy-grouppolicypresentationtext.md)|
|[Criar groupPolicyPresentationText](../api/intune-grouppolicy-grouppolicypresentationtext-create.md)|[groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md)|Crie um novo [objeto groupPolicyPresentationText.](../resources/intune-grouppolicy-grouppolicypresentationtext.md)|
|[Excluir groupPolicyPresentationText](../api/intune-grouppolicy-grouppolicypresentationtext-delete.md)|Nenhum|Exclui um [groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md).|
|[Atualizar groupPolicyPresentationText](../api/intune-grouppolicy-grouppolicypresentationtext-update.md)|[groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md)|Atualize as propriedades de [um objeto groupPolicyPresentationText.](../resources/intune-grouppolicy-grouppolicypresentationtext.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|rótulo|Cadeia de Caracteres|Rótulo de texto localizado para qualquer entidade de apresentação. O valor padrão é vazio. Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|Cadeia de caracteres|Chave da entidade. Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que a entidade foi modificada pela última vez. Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|A definição de política de grupo associada à apresentação. Herdado [de groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|

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



