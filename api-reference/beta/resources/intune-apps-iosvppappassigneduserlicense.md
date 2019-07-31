---
title: tipo de recurso iosVppAppAssignedUserLicense
description: atribuição de licença de usuário do programa de compra de volume iOS. Essa classe não oferece suporte para Criar, Excluir ou Atualizar.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9e259c1b31d1b61fe3c9a3508d52160ddbe0c4fd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005475"
---
# <a name="iosvppappassigneduserlicense-resource-type"></a>tipo de recurso iosVppAppAssignedUserLicense

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

atribuição de licença de usuário do programa de compra de volume iOS. Essa classe não oferece suporte para Criar, Excluir ou Atualizar.


Herda de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar iosVppAppAssignedUserLicenses](../api/intune-apps-iosvppappassigneduserlicense-list.md)|coleção [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)|Listar Propriedades e relações dos objetos [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) .|
|[Obter iosVppAppAssignedUserLicense](../api/intune-apps-iosvppappassigneduserlicense-get.md)|[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)|Leia as propriedades e as relações do objeto [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) .|
|[Criar iosVppAppAssignedUserLicense](../api/intune-apps-iosvppappassigneduserlicense-create.md)|[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)|Criar um novo objeto [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) .|
|[Excluir iosVppAppAssignedUserLicense](../api/intune-apps-iosvppappassigneduserlicense-delete.md)|Nenhum|Exclui [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md).|
|[Atualizar iosVppAppAssignedUserLicense](../api/intune-apps-iosvppappassigneduserlicense-update.md)|[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)|Atualiza as propriedades de um objeto [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|useremailaddress|String|O endereço de email do usuário. Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userId|String|A ID do usuário. Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userName|Cadeia de caracteres|O nome de usuário. Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userPrincipalName|String|O nome da entidade de segurança do usuário. Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppAppAssignedUserLicense"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedUserLicense",
  "id": "String (identifier)",
  "userEmailAddress": "String",
  "userId": "String",
  "userName": "String",
  "userPrincipalName": "String"
}
```





