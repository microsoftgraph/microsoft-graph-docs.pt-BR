---
title: Tipo de recurso managedMobileApp
description: O identificador da implantação de um aplicativo.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1c020166da2fb8e33d9649935f89ef22e556e7d8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819696"
---
# <a name="managedmobileapp-resource-type"></a>Tipo de recurso managedMobileApp

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

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
|id|Cadeia de caracteres|Chave da entidade.|
|version|Cadeia de caracteres|Versão da entidade.|

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



