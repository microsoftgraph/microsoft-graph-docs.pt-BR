---
title: tipo de recurso de cartToClassAssociation
description: CartToClassAssociation para associar carrinhos de dispositivo salas.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b832e4597b15f062289a086d068ea3da71d9f66a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395689"
---
# <a name="carttoclassassociation-resource-type"></a>tipo de recurso de cartToClassAssociation

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

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




