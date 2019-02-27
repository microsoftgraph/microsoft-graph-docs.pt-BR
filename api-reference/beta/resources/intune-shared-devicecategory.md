---
title: Tipo de recurso deviceCategory
description: Essas categorias podem então ser aplicadas a um dispositivo no console do Intune Azure ou selecionadas por um usuário durante o registro de um dispositivo. Você pode filtrar relatórios e criar grupos de dispositivos dinâmicos do Azure Active Directory com base em categorias de dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 75fb11ef3b734e6d5d0490be1abc3c5399433a70
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174549"
---
# <a name="devicecategory-resource-type"></a>Tipo de recurso deviceCategory

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

As categorias de dispositivo fornecem uma maneira de organizar seus dispositivos. Usando categorias de dispositivos, os administradores da empresa podem definir categorias exclusivas que fazem sentido para sua empresa.Essas categorias podem então ser aplicadas a um dispositivo no console do Intune Azure ou selecionadas por um usuário durante o registro de um dispositivo. Você pode filtrar relatórios e criar grupos de dispositivos dinâmicos do Azure Active Directory com base em categorias de dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceCategories](../api/intune-shared-devicecategory-list.md)|Coleção [deviceCategory](../resources/intune-shared-devicecategory.md)|Lista propriedades e relações dos objetos [deviceCategory](../resources/intune-shared-devicecategory.md).|
|[Obter deviceCategory](../api/intune-shared-devicecategory-get.md)|[deviceCategory](../resources/intune-shared-devicecategory.md)|Propriedades de leitura e relações do objeto [deviceCategory](../resources/intune-shared-devicecategory.md).|
|[Criar deviceCategory](../api/intune-shared-devicecategory-create.md)|[deviceCategory](../resources/intune-shared-devicecategory.md)|Cria um novo objeto [deviceCategory](../resources/intune-shared-devicecategory.md).|
|[Excluir deviceCategory](../api/intune-shared-devicecategory-delete.md)|Nenhuma|Exclui um [deviceCategory](../resources/intune-shared-devicecategory.md).|
|[Atualizar deviceCategory](../api/intune-shared-devicecategory-update.md)|[deviceCategory](../resources/intune-shared-devicecategory.md)|Atualiza as propriedades de um objeto [deviceCategory](../resources/intune-shared-devicecategory.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo da categoria do dispositivo. Somente leitura.|
|**Integração**|
|displayName|String|Nome de exibição da categoria de dispositivo.|
|description|Cadeia de caracteres|Descrição opcional da categoria do dispositivo.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```



