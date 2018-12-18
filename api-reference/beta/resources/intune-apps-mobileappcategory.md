---
title: Tipo de recurso mobileAppCategory
description: Contém as propriedades para uma única categoria de aplicativo do Intune.
author: tfitzmac
ms.openlocfilehash: f40e9a24269d276c89d770acb0d772a7bdf94c51
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340758"
---
# <a name="mobileappcategory-resource-type"></a>Tipo de recurso mobileAppCategory

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

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





