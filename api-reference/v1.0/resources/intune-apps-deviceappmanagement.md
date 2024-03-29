---
title: Tipo de recurso deviceAppManagement
description: Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de aplicativos de dispositivos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a55275a47a3e4fa4d42576c0ecefabdc61a68e9f
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66732489"
---
# <a name="deviceappmanagement-resource-type"></a>Tipo de recurso deviceAppManagement

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de aplicativos de dispositivos.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter deviceAppManagement](../api/intune-apps-deviceappmanagement-get.md)|[deviceAppManagement](../resources/intune-apps-deviceappmanagement.md)|Ler propriedades e relações de objetos de [deviceAppManagement](../resources/intune-apps-deviceappmanagement.md).|
|[Atualizar deviceAppManagement](../api/intune-apps-deviceappmanagement-update.md)|[deviceAppManagement](../resources/intune-apps-deviceappmanagement.md)|Atualizar as propriedades de um objeto de [deviceAppManagement](../resources/intune-apps-deviceappmanagement.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|mobileApps|Coleção [mobileApp](../resources/intune-apps-mobileapp.md)|Os aplicativos móveis.|
|mobileAppCategories|Coleção [mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|As categorias dos aplicativos móveis.|
|mobileAppConfigurations|Coleção [managedDeviceMobileAppConfiguration](../resources/intune-apps-manageddevicemobileappconfiguration.md)|As configurações de aplicativos móveis de gerenciamento de dispositivos.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)"
}
```





