---
title: Tipo de recurso deviceManagementUserRightsLocalUserOrGroup
description: Representa informações para um usuário ou grupo local usado para a configuração de direitos do usuário.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3fe52f8a0a6460f3cac12bf535526ab73d4e58340d31339b2c78baea728964ca
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54148222"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a>Tipo de recurso deviceManagementUserRightsLocalUserOrGroup

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa informações para um usuário ou grupo local usado para a configuração de direitos do usuário.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|nome|Cadeia de caracteres|O nome desse usuário ou grupo local.|
|description|Cadeia de caracteres|Descrição do administrador deste usuário ou grupo local.|
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




