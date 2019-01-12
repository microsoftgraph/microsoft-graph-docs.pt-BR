---
title: tipo de recurso de cartToClassAssociation
description: CartToClassAssociation para associar carrinhos de dispositivo salas.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 38d9b940dd3e7a5450854f29ba69b2eac69e2a45
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27943932"
---
# <a name="carttoclassassociation-resource-type"></a>tipo de recurso de cartToClassAssociation

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

CartToClassAssociation para associar carrinhos de dispositivo salas.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista cartToClassAssociations](../api/intune-deviceconfig-carttoclassassociation-list.md)|coleção [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|Lista as propriedades e os relacionamentos dos objetos [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) .|
|[Obter cartToClassAssociation](../api/intune-deviceconfig-carttoclassassociation-get.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|Leia as propriedades e os relacionamentos do objeto [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) .|
|[Criar cartToClassAssociation](../api/intune-deviceconfig-carttoclassassociation-create.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|Crie um novo objeto de [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) .|
|[Excluir cartToClassAssociation](../api/intune-deviceconfig-carttoclassassociation-delete.md)|Nenhum|Exclui um [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md).|
|[Atualizar cartToClassAssociation](../api/intune-deviceconfig-carttoclassassociation-update.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|Atualize as propriedades de um objeto [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado.|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto.|
|version|Int32|Versão do CartToClassAssociation.|
|displayName|String|O administrador forneceu o nome da Configuração do dispositivo.|
|description|String|Admin fornecido descrição do que o CartToClassAssociation.|
|deviceCartIds|String collection|Identificadores de carrinhos de dispositivo a ser associado a classes.|
|classroomIds|String collection|Identificadores de salas a ser associado ao dispositivo carrinhos de.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cartToClassAssociation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cartToClassAssociation",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024,
  "displayName": "String",
  "description": "String",
  "deviceCartIds": [
    "String"
  ],
  "classroomIds": [
    "String"
  ]
}
```





