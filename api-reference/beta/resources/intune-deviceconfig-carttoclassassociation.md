---
title: tipo de recurso cartToClassAssociation
description: CartToClassAssociation para associação de carrinhos de dispositivos com salas de aula.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5aaced5f6c5959b4113ae5d6ff3cbbfecb0a1ba1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081619"
---
# <a name="carttoclassassociation-resource-type"></a>tipo de recurso cartToClassAssociation

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

CartToClassAssociation para associação de carrinhos de dispositivos com salas de aula.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar cartToClassAssociations](../api/intune-deviceconfig-carttoclassassociation-list.md)|coleção [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|Listar Propriedades e relações dos objetos [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) .|
|[Obter cartToClassAssociation](../api/intune-deviceconfig-carttoclassassociation-get.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|Leia as propriedades e as relações do objeto [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) .|
|[Criar cartToClassAssociation](../api/intune-deviceconfig-carttoclassassociation-create.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|Criar um novo objeto [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) .|
|[Excluir cartToClassAssociation](../api/intune-deviceconfig-carttoclassassociation-delete.md)|Nenhum|Exclui [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md).|
|[Atualizar cartToClassAssociation](../api/intune-deviceconfig-carttoclassassociation-update.md)|[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)|Atualiza as propriedades de um objeto [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|createdDateTime|DateTimeOffset|DateTime em que o objeto foi criado.|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto.|
|versão|Int32|Versão do CartToClassAssociation.|
|displayName|Cadeia de caracteres|O administrador forneceu o nome da Configuração do dispositivo.|
|description|Cadeia de caracteres|Descrição fornecida pelo administrador do CartToClassAssociation.|
|deviceCartIds|Coleção String|Identificadores de carrinhos de dispositivos a serem associados às classes.|
|classroomIds|Coleção String|Identificadores de salas de aula a serem associadas a carrinhos de dispositivos.|

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






