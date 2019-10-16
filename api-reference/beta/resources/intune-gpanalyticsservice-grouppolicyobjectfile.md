---
title: tipo de recurso groupPolicyObjectFile
description: O arquivo de objeto da diretiva de grupo carregado por administrador.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b28ba6364f3261a7cd341870de402dc9332c87b4
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539194"
---
# <a name="grouppolicyobjectfile-resource-type"></a>tipo de recurso groupPolicyObjectFile

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O arquivo de objeto da diretiva de grupo carregado por administrador.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|ouDistinguishedName|Cadeia de caracteres|O nome diferenciado da OU.|
|content|Cadeia de caracteres|O conteúdo do arquivo do objeto de diretiva de grupo.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.groupPolicyObjectFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyObjectFile",
  "ouDistinguishedName": "String",
  "content": "String"
}
```



