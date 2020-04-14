---
title: Tipo de recurso mobileAppCategory
description: Contém as propriedades para uma única categoria de aplicativo do Intune.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: aeca0599e3793491763796cd210ebd3dcfd80f1d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43458587"
---
# <a name="mobileappcategory-resource-type"></a>Tipo de recurso mobileAppCategory

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Contém as propriedades para uma única categoria de aplicativo do Intune.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar mobileAppCategories](../api/intune-apps-mobileappcategory-list.md)|Conjunto [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Listar propriedades e as relações de objetos de [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).|
|[Obter mobileAppCategory](../api/intune-apps-mobileappcategory-get.md)|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Ler propriedades e relações de objetos de [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).|
|[Criar mobileAppCategory](../api/intune-apps-mobileappcategory-create.md)|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Criar um novo objeto de [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).|
|[Excluir mobileAppCategory](../api/intune-apps-mobileappcategory-delete.md)|Nenhum|Excluir uma [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).|
|[Atualizar mobileAppCategory](../api/intune-apps-mobileappcategory-update.md)|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|Atualizar as propriedades de um objeto de [mobileAppCategory](../resources/intune-apps-mobileappcategory.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|A chave da entidade.|
|displayName|Cadeia de caracteres|O nome da categoria do aplicativo.|
|lastModifiedDateTime|DateTimeOffset|A data e hora que a mobileAppCategory foi modificada pela última vez.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```



