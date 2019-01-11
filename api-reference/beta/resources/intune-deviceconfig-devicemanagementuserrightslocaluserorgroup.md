---
title: tipo de recurso de deviceManagementUserRightsLocalUserOrGroup
description: Representa informações para um usuário ou grupo local usado para a definição de direitos de usuário.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d795e2b259c71612b1d0720796b6ad76145bb36d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885734"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a>tipo de recurso de deviceManagementUserRightsLocalUserOrGroup

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Representa informações para um usuário ou grupo local usado para a definição de direitos de usuário.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|name|Cadeia de caracteres|O nome deste usuário local ou grupo.|
|description|Cadeia de caracteres|Descrição do Admin este usuário ou grupo local.|
|securityIdentifier|Cadeia de caracteres|O identificador de segurança deste usuário local ou grupo (por exemplo, * S-1-5-32-544).|

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





