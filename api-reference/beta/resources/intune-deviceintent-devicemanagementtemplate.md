---
title: tipo de recurso deviceManagementTemplate
description: Entidade que representa uma coleção definida de configurações de dispositivo
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a55e4426f37f0261f5adbd1ac4830de6ede3e3ed
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575853"
---
# <a name="devicemanagementtemplate-resource-type"></a>tipo de recurso deviceManagementTemplate

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade que representa uma coleção definida de configurações de dispositivo

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementTemplates](../api/intune-deviceintent-devicemanagementtemplate-list.md)|coleção [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|Listar Propriedades e relações dos objetos [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) .|
|[Obter deviceManagementTemplate](../api/intune-deviceintent-devicemanagementtemplate-get.md)|[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|Leia as propriedades e as relações do objeto [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) .|
|[Criar deviceManagementTemplate](../api/intune-deviceintent-devicemanagementtemplate-create.md)|[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|Criar um novo objeto [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) .|
|[Excluir deviceManagementTemplate](../api/intune-deviceintent-devicemanagementtemplate-delete.md)|Nenhum|Exclui [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md).|
|[Atualizar deviceManagementTemplate](../api/intune-deviceintent-devicemanagementtemplate-update.md)|[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|Atualiza as propriedades de um objeto [deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md) .|
|[ação createInstance](../api/intune-deviceintent-devicemanagementtemplate-createinstance.md)|[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID do modelo|
|displayName|String|O nome de exibição do modelo|
|description|String|A descrição do modelo|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|settings|coleção [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|Coleção de todas as configurações que este modelo tem|
|categories|coleção [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)|Conjunto de categorias de configuração no modelo|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```





