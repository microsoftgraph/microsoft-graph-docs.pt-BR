---
title: Tipo de recurso deviceCategory
description: Categorias de dispositivo fornecem uma maneira de organizar seus dispositivos. Usando categorias de dispositivo, os administradores podem definir suas próprias categorias que fazem sentido para suas empresas. Essas categorias podem então ser aplicadas a um dispositivo no console do Intune Azure ou selecionadas por um usuário durante o registro de um dispositivo. Você pode filtrar relatórios e criar grupos de dispositivos dinâmicos do Azure Active Directory com base em categorias de dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5def5ee6c6a97e91c9255a9808db7fc6b2fa07fc
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751772"
---
# <a name="devicecategory-resource-type"></a>Tipo de recurso deviceCategory

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Categorias de dispositivo fornecem uma maneira de organizar seus dispositivos. Usando categorias de dispositivo, os administradores podem definir suas próprias categorias que fazem sentido para suas empresas. Essas categorias podem então ser aplicadas a um dispositivo no console do Intune Azure ou selecionadas por um usuário durante o registro de um dispositivo. Você pode filtrar relatórios e criar grupos de dispositivos dinâmicos do Azure Active Directory com base em categorias de dispositivo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceCategories](../api/intune-onboarding-devicecategory-list.md)|Coleção [deviceCategory](../resources/intune-onboarding-devicecategory.md)|Lista propriedades e relações dos objetos [deviceCategory](../resources/intune-onboarding-devicecategory.md).|
|[Obter deviceCategory](../api/intune-onboarding-devicecategory-get.md)|[deviceCategory](../resources/intune-onboarding-devicecategory.md)|Propriedades de leitura e relações do objeto [deviceCategory](../resources/intune-onboarding-devicecategory.md).|
|[Criar deviceCategory](../api/intune-onboarding-devicecategory-create.md)|[deviceCategory](../resources/intune-onboarding-devicecategory.md)|Cria um novo objeto [deviceCategory](../resources/intune-onboarding-devicecategory.md).|
|[Excluir deviceCategory](../api/intune-onboarding-devicecategory-delete.md)|Nenhuma|Exclui um [deviceCategory](../resources/intune-onboarding-devicecategory.md).|
|[Atualizar deviceCategory](../api/intune-onboarding-devicecategory-update.md)|[deviceCategory](../resources/intune-onboarding-devicecategory.md)|Atualiza as propriedades de um objeto [deviceCategory](../resources/intune-onboarding-devicecategory.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|O identificador exclusivo da categoria do dispositivo. Somente leitura.|
|displayName|String|Nome de exibição da categoria de dispositivo.|
|description|String|Descrição opcional da categoria do dispositivo.|

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




