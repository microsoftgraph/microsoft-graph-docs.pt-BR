---
title: Tipo de recurso deviceCategory
description: Essas categorias podem então ser aplicadas a um dispositivo no console do Intune Azure ou selecionadas por um usuário durante o registro de um dispositivo. Você pode filtrar relatórios e criar grupos de dispositivos dinâmicos do Azure Active Directory com base em categorias de dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 067e7894cc5c5daa4cd73c5bb5ba88f66b283366
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732224"
---
# <a name="devicecategory-resource-type"></a>Tipo de recurso deviceCategory

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Categorias de dispositivo fornecem uma maneira de organizar seus dispositivos. Usando categorias de dispositivo, os administradores podem definir suas próprias categorias que fazem sentido para suas empresas. Essas categorias podem então ser aplicadas a um dispositivo no console do Intune Azure ou selecionadas por um usuário durante o registro de um dispositivo. Você pode filtrar relatórios e criar grupos de dispositivos dinâmicos do Azure Active Directory com base em categorias de dispositivo.

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar coleção deviceCategories](../api/intune-shared-devicecategory-list.md)|Lista propriedades e relações dos objetos [deviceCategory](../resources/intune-shared-devicecategory.md).|
|[Obter deviceCategory](../api/intune-shared-devicecategory-get.md)|Propriedades de leitura e relações do objeto [deviceCategory](../resources/intune-shared-devicecategory.md).|
|[Criar deviceCategory](../api/intune-shared-devicecategory-create.md)|Cria um novo objeto [deviceCategory](../resources/intune-shared-devicecategory.md).|
|[Excluir deviceCategory](../api/intune-shared-devicecategory-delete.md).|
|[Atualizar deviceCategory](../api/intune-shared-devicecategory-update.md)|Atualiza as propriedades de um objeto [deviceCategory](../resources/intune-shared-devicecategory.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo da categoria do dispositivo. Somente leitura.|
|**Integração**|
|displayName|Cadeia de caracteres|Nome de exibição da categoria de dispositivo.|
|descrição|Cadeia de caracteres|Descrição opcional da categoria do dispositivo.|

## <a name="relationships"></a>Relações
Nenhuma

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









