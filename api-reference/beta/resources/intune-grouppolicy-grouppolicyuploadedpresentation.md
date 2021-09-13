---
title: Tipo de recurso groupPolicyUploadedPresentation
description: A entidade base para a apresentação de exibição de qualquer uma das opções adicionais em uma definição de política de grupo.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: acaf9f6bfc440327ed7c2b08b0e00cea36ffef9d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59046747"
---
# <a name="grouppolicyuploadedpresentation-resource-type"></a>Tipo de recurso groupPolicyUploadedPresentation

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade base para a apresentação de exibição de qualquer uma das opções adicionais em uma definição de política de grupo.


Herda de [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar groupPolicyUploadedPresentations](../api/intune-grouppolicy-grouppolicyuploadedpresentation-list.md)|[coleção groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md)|Listar propriedades e relações dos [objetos groupPolicyUploadedPresentation.](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md)|
|[Obter groupPolicyUploadedPresentation](../api/intune-grouppolicy-grouppolicyuploadedpresentation-get.md)|[groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md)|Leia propriedades e relações do [objeto groupPolicyUploadedPresentation.](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md)|
|[Criar groupPolicyUploadedPresentation](../api/intune-grouppolicy-grouppolicyuploadedpresentation-create.md)|[groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md)|Crie um novo [objeto groupPolicyUploadedPresentation.](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md)|
|[Excluir groupPolicyUploadedPresentation](../api/intune-grouppolicy-grouppolicyuploadedpresentation-delete.md)|Nenhum|Exclui um [groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md).|
|[Atualizar groupPolicyUploadedPresentation](../api/intune-grouppolicy-grouppolicyuploadedpresentation-update.md)|[groupPolicyUploadedPresentation](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md)|Atualize as propriedades de [um objeto groupPolicyUploadedPresentation.](../resources/intune-grouppolicy-grouppolicyuploadedpresentation.md)|

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
  "@odata.type": "microsoft.graph.groupPolicyUploadedPresentation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedPresentation",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```



