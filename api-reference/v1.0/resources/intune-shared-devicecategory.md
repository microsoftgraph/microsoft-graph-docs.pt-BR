---
title: Tipo de recurso deviceCategory
description: Essas categorias podem então ser aplicadas a um dispositivo no console do Intune Azure ou selecionadas por um usuário durante o registro de um dispositivo. Você pode filtrar relatórios e criar grupos de dispositivos dinâmicos do Azure Active Directory com base em categorias de dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0267e547d9ee9f3846fa2f44596638d586f3158d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968558"
---
# <a name="devicecategory-resource-type"></a>Tipo de recurso deviceCategory

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Categorias de dispositivo fornecem uma maneira de organizar seus dispositivos. Usando categorias de dispositivo, os administradores podem definir suas próprias categorias que fazem sentido para suas empresas.Essas categorias podem então ser aplicadas a um dispositivo no console do Intune Azure ou selecionadas por um usuário durante o registro de um dispositivo. Você pode filtrar relatórios e criar grupos de dispositivos dinâmicos do Azure Active Directory com base em categorias de dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|Coleção da [lista deviceCategories](../api/intune-shared-devicecategory-list.md)|Lista propriedades e relações dos objetos [deviceCategory](../resources/intune-shared-devicecategory.md).|
|[Obter deviceCategory](../api/intune-shared-devicecategory-get.md)|Propriedades de leitura e relações do objeto [deviceCategory](../resources/intune-shared-devicecategory.md).|
|[Criar deviceCategory](../api/intune-shared-devicecategory-create.md)|Cria um novo objeto [deviceCategory](../resources/intune-shared-devicecategory.md).|
|[Excluir deviceCategory](../api/intune-shared-devicecategory-delete.md).|
|[Atualizar deviceCategory](../api/intune-shared-devicecategory-update.md)|Atualiza as propriedades de um objeto [deviceCategory](../resources/intune-shared-devicecategory.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo da categoria do dispositivo. Somente leitura.|
|**Inclusão**|
|displayName|Cadeia de caracteres|Nome de exibição da categoria de dispositivo.|
|description|Cadeia de caracteres|Descrição opcional da categoria do dispositivo.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceCategory"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```



