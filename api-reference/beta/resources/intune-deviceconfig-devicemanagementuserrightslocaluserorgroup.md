---
title: tipo de recurso de deviceManagementUserRightsLocalUserOrGroup
description: Representa informações para um usuário ou grupo local usado para a definição de direitos de usuário.
author: tfitzmac
ms.openlocfilehash: baabd2f3bb9e3bce44d172cd83f61f57c5c2c98d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303728"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a>tipo de recurso de deviceManagementUserRightsLocalUserOrGroup

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Representa informações para um usuário ou grupo local usado para a definição de direitos de usuário.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|name|String|O nome deste usuário local ou grupo.|
|description|String|Descrição do Admin este usuário ou grupo local.|
|securityIdentifier|String|O identificador de segurança deste usuário local ou grupo (por exemplo, * S-1-5-32-544).|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
  "name": "String",
  "description": "String",
  "securityIdentifier": "String"
}
```





