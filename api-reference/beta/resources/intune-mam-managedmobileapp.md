---
title: Tipo de recurso managedMobileApp
description: O identificador da implantação de um aplicativo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 145287fe1b5cc75d5b12802d2dd5d30bcbfb7bd9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373025"
---
# <a name="managedmobileapp-resource-type"></a>Tipo de recurso managedMobileApp

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

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
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "String (identifier)",
  "version": "String"
}
```



