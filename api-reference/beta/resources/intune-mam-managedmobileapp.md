---
title: Tipo de recurso managedMobileApp
description: O identificador da implantação de um aplicativo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1a10bb4a8aac77a87919d26ea1b08adc49689151
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155899"
---
# <a name="managedmobileapp-resource-type"></a>Tipo de recurso managedMobileApp

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O identificador da implantação de um aplicativo.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar managedMobileApps](../api/intune-mam-managedmobileapp-list.md)|Conjunto [managedMobileApp](../resources/intune-mam-managedmobileapp.md)|Listar propriedades e relações de objetos de [managedMobileApp](../resources/intune-mam-managedmobileapp.md).|
|[Obter managedMobileApp](../api/intune-mam-managedmobileapp-get.md)|[managedMobileApp](../resources/intune-mam-managedmobileapp.md)|Ler propriedades e relações de objetos de [managedMobileApp](../resources/intune-mam-managedmobileapp.md).|
|[Criar managedMobileApp](../api/intune-mam-managedmobileapp-create.md)|[managedMobileApp](../resources/intune-mam-managedmobileapp.md)|Criar um novo objeto de[managedMobileApp](../resources/intune-mam-managedmobileapp.md).|
|[Excluir managedMobileApp](../api/intune-mam-managedmobileapp-delete.md)|Nenhum|Excluir [managedMobileApp](../resources/intune-mam-managedmobileapp.md).|
|[Atualizar managedMobileApp](../api/intune-mam-managedmobileapp-update.md)|[managedMobileApp](../resources/intune-mam-managedmobileapp.md)|Atualizar as propriedades de um objeto de [managedMobileApp](../resources/intune-mam-managedmobileapp.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|mobileAppIdentifier|[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)|O identificador de um aplicativo com seu tipo de sistema operacional.|
|id|String|Chave da entidade.|
|versão|String|Versão da entidade.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedMobileApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.windowsAppIdentifier",
    "windowsAppId": "String"
  },
  "id": "String (identifier)",
  "version": "String"
}
```




