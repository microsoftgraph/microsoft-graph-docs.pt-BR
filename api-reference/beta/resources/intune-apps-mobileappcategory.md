---
title: Tipo de recurso mobileAppCategory
description: Contém as propriedades para uma única categoria de aplicativo do Intune.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1878b5af99f1dc87eb3e6659d0d1101b379a526e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59087027"
---
# <a name="mobileappcategory-resource-type"></a>Tipo de recurso mobileAppCategory

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

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
|id|Cadeia de caracteres|A chave da entidade.|
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



