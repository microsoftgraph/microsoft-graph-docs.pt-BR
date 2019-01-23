---
title: Tipo de recurso deviceCategory
description: Essas categorias podem então ser aplicadas a um dispositivo no console do Intune Azure ou selecionadas por um usuário durante o registro de um dispositivo. Você pode filtrar relatórios e criar grupos de dispositivos dinâmicos do Azure Active Directory com base em categorias de dispositivo.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b7470f6cf0193474bfaff4f7444ed3df1d9453a5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418859"
---
# <a name="devicecategory-resource-type"></a>Tipo de recurso deviceCategory

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Categorias de dispositivos fornecem uma maneira de organizar seus dispositivos. Usando categorias de dispositivo, administradores de empresa podem definir categorias exclusivas que faz sentido para sua empresa.Essas categorias podem então ser aplicadas a um dispositivo no console do Intune Azure ou selecionadas por um usuário durante o registro de um dispositivo. Você pode filtrar relatórios e criar grupos de dispositivos dinâmicos do Azure Active Directory com base em categorias de dispositivo.

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
|id|Cadeia de caracteres|O identificador exclusivo da categoria do dispositivo. Somente leitura.|
|**Inclusão**|
|displayName|Cadeia de caracteres|Nome de exibição da categoria de dispositivo.|
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



