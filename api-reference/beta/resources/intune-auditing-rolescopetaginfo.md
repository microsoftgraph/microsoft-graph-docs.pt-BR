---
title: Tipo de recurso roleScopeTagInfo
description: Uma classe que contém as propriedades do objeto de marca de escopo de função.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3a3d3a5461b01ad5a0a0688bb02e7b1080c97746
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59075778"
---
# <a name="rolescopetaginfo-resource-type"></a>Tipo de recurso roleScopeTagInfo

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe que contém as propriedades do objeto de marca de escopo de função.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|Cadeia de caracteres|Nome de exibição da marca de escopo.|
|roleScopeTagId|Cadeia de caracteres|ID da Marca de Escopo.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.roleScopeTagInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.roleScopeTagInfo",
  "displayName": "String",
  "roleScopeTagId": "String"
}
```



