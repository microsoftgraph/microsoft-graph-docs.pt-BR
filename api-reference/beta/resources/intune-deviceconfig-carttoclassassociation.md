---
title: Tipo de recurso cartToClassAssociation
description: CartToClassAssociation para associar carrinhos de dispositivo a salas de aula.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 421f00600febc567f10b754e86e061aa5e57fa29
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58779134"
---
# <a name="carttoclassassociation-resource-type"></a>Tipo de recurso cartToClassAssociation

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

CartToClassAssociation para associar carrinhos de dispositivo a salas de aula.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar cartToClassAssociations](../api/intune-deviceconfig-carttoclassassociation-list.md)|[Coleção cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|Listar propriedades e relações dos [objetos cartToClassAssociation.](../resources/intune-deviceconfig-carttoclassassociation.md)|
|[Obter cartToClassAssociation](../api/intune-deviceconfig-carttoclassassociation-get.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|Leia propriedades e relações do [objeto cartToClassAssociation.](../resources/intune-deviceconfig-carttoclassassociation.md)|
|[Criar cartToClassAssociation](../api/intune-deviceconfig-carttoclassassociation-create.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|Crie um novo [objeto cartToClassAssociation.](../resources/intune-deviceconfig-carttoclassassociation.md)|
|[Excluir cartToClassAssociation](../api/intune-deviceconfig-carttoclassassociation-delete.md)|Nenhum(a)|Exclui um [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md).|
|[Atualizar cartToClassAssociation](../api/intune-deviceconfig-carttoclassassociation-update.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|Atualize as propriedades de um [objeto cartToClassAssociation.](../resources/intune-deviceconfig-carttoclassassociation.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado.|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto.|
|versão|Int32|Versão do CartToClassAssociation.|
|displayName|Cadeia de caracteres|O administrador forneceu o nome da Configuração do dispositivo.|
|descrição|Cadeia de caracteres|O administrador forneceu a descrição do CartToClassAssociation.|
|deviceCartIds|Coleção de cadeias de caracteres|Identificadores de carrinhos de dispositivo a serem associados a classes.|
|classroomIds|Coleção de cadeias de caracteres|Identificadores de salas de aula a serem associadas a carrinhos de dispositivo.|

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



