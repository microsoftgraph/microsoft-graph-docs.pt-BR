---
title: Tipo de recurso groupPolicyPresentationValue
description: A entidade de valor de apresentação base que armazena o valor de uma apresentação de política de grupo único.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8783cce5c6175a18cbc490743479ca5e1c8eb17b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59085977"
---
# <a name="grouppolicypresentationvalue-resource-type"></a>Tipo de recurso groupPolicyPresentationValue

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A entidade de valor de apresentação base que armazena o valor de uma apresentação de política de grupo único.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar groupPolicyPresentationValues](../api/intune-grouppolicy-grouppolicypresentationvalue-list.md)|[coleção groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|Listar propriedades e relações dos [objetos groupPolicyPresentationValue.](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|[Obter groupPolicyPresentationValue](../api/intune-grouppolicy-grouppolicypresentationvalue-get.md)|[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|Leia propriedades e relações do [objeto groupPolicyPresentationValue.](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|[Criar groupPolicyPresentationValue](../api/intune-grouppolicy-grouppolicypresentationvalue-create.md)|[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|Crie um novo [objeto groupPolicyPresentationValue.](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|
|[Excluir groupPolicyPresentationValue](../api/intune-grouppolicy-grouppolicypresentationvalue-delete.md)|Nenhum|Exclui um [groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md).|
|[Atualizar groupPolicyPresentationValue](../api/intune-grouppolicy-grouppolicypresentationvalue-update.md)|[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|Atualize as propriedades de [um objeto groupPolicyPresentationValue.](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que o objeto foi modificado pela última vez.|
|createdDateTime|DateTimeOffset|A data e a hora em que o objeto foi criado.|
|id|Cadeia de caracteres|Chave da entidade.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|definitionValue|[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|O valor de definição de política de grupo associado ao valor de apresentação.|
|presentation|[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|A apresentação da política de grupo associada ao valor de apresentação.|

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



