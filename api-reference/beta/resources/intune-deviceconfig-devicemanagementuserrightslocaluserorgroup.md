---
title: Tipo de recurso deviceManagementUserRightsLocalUserOrGroup
description: Representa informações para um usuário ou grupo local usado para a configuração de direitos do usuário.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bb8dd01d090c5d0aaef133b5e5b6367f5acdd278
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59069226"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a>Tipo de recurso deviceManagementUserRightsLocalUserOrGroup

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa informações para um usuário ou grupo local usado para a configuração de direitos do usuário.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|nome|String|O nome desse usuário ou grupo local.|
|description|String|Descrição do administrador deste usuário ou grupo local.|
|securityIdentifier|Cadeia de Caracteres|O identificador de segurança deste usuário ou grupo local (por exemplo, *S-1-5-32-544).|

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



