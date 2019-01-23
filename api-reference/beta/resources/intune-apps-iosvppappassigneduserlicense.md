---
title: tipo de recurso de iosVppAppAssignedUserLicense
description: iOS atribuição de licença de usuário do programa de compra do Volume. Essa classe não oferece suporte para Criar, Excluir ou Atualizar.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3f777ac91097bfd0ad25437702922ebe12ce4dac
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418453"
---
# <a name="iosvppappassigneduserlicense-resource-type"></a>tipo de recurso de iosVppAppAssignedUserLicense

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

iOS atribuição de licença de usuário do programa de compra do Volume. Essa classe não oferece suporte para Criar, Excluir ou Atualizar.


Herda de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Lista iosVppAppAssignedUserLicenses](../api/intune-apps-iosvppappassigneduserlicense-list.md)|coleção [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)|Lista as propriedades e os relacionamentos dos objetos [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) .|
|[Obter iosVppAppAssignedUserLicense](../api/intune-apps-iosvppappassigneduserlicense-get.md)|[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)|Leia as propriedades e os relacionamentos do objeto [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) .|
|[Criar iosVppAppAssignedUserLicense](../api/intune-apps-iosvppappassigneduserlicense-create.md)|[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)|Crie um novo objeto de [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) .|
|[Excluir iosVppAppAssignedUserLicense](../api/intune-apps-iosvppappassigneduserlicense-delete.md)|Nenhum|Exclui um [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md).|
|[Atualizar iosVppAppAssignedUserLicense](../api/intune-apps-iosvppappassigneduserlicense-update.md)|[iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md)|Atualize as propriedades de um objeto [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave da entidade. Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userEmailAddress|String|O endereço de email do usuário. Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
|userId|String|ID do usuário. Herdado de [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)|
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




