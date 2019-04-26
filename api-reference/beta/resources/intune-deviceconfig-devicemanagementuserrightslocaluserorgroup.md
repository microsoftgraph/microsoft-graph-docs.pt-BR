---
title: tipo de recurso deviceManagementUserRightsLocalUserOrGroup
description: Representa informações de um usuário ou grupo local usado para a configuração de direitos do usuário.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cfdb49ef0b98e3d76d092b1ebf9574d6df8c47d9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567197"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a>tipo de recurso deviceManagementUserRightsLocalUserOrGroup

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa informações de um usuário ou grupo local usado para a configuração de direitos do usuário.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|name|String|O nome desse usuário ou grupo local.|
|description|String|Descrição do administrador desse usuário ou grupo local.|
|securityIdentifier|String|O identificador de segurança desse usuário ou grupo local (por exemplo, * S-1-5-32-544).|

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





