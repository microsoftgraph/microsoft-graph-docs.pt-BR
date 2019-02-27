---
title: tipo de recurso iosVppAppAssignedDeviceLicense
description: atribuição de licença de dispositivo do iOS Volume Purchase Program. Essa classe não oferece suporte para Criar, Excluir ou Atualizar.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 56e41bdabc8b6585fe5b003d28eaa4259046f662
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174619"
---
# <a name="iosvppappassigneddevicelicense-resource-type"></a>tipo de recurso iosVppAppAssignedDeviceLicense

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

atribuição de licença de dispositivo do iOS Volume Purchase Program. Essa classe não oferece suporte para Criar, Excluir ou Atualizar.


Herda de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar iosVppAppAssignedDeviceLicenses](../api/intune-apps-iosvppappassigneddevicelicense-list.md)|coleção [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)|Listar Propriedades e relações dos objetos [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) .|
|[Obter iosVppAppAssignedDeviceLicense](../api/intune-apps-iosvppappassigneddevicelicense-get.md)|[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)|Leia as propriedades e as relações do objeto [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) .|
|[Criar iosVppAppAssignedDeviceLicense](../api/intune-apps-iosvppappassigneddevicelicense-create.md)|[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)|Criar um novo objeto [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) .|
|[Excluir iosVppAppAssignedDeviceLicense](../api/intune-apps-iosvppappassigneddevicelicense-delete.md)|Nenhum|Exclui [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md).|
|[Atualizar iosVppAppAssignedDeviceLicense](../api/intune-apps-iosvppappassigneddevicelicense-update.md)|[iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md)|Atualiza as propriedades de um objeto [iosVppAppAssignedDeviceLicense](../resources/intune-apps-iosvppappassigneddevicelicense.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userEmailAddress|String|O endereço de email do usuário. Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userId|String|A ID de usuário. Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userName|String|O nome de usuário. Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userPrincipalName|String|O nome da entidade de segurança do usuário. Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|managedDeviceId|String|A ID do dispositivo gerenciado.|
|deviceName|Cadeia de caracteres|O nome do dispositivo.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppAppAssignedDeviceLicense"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedDeviceLicense",
  "id": "String (identifier)",
  "userEmailAddress": "String",
  "userId": "String",
  "userName": "String",
  "userPrincipalName": "String",
  "managedDeviceId": "String",
  "deviceName": "String"
}
```




