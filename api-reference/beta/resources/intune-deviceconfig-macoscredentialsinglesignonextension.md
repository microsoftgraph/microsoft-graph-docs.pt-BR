---
title: tipo de recurso macOSCredentialSingleSignOnExtension
description: Representa um perfil de extensão de logon único de tipo de credencial para dispositivos macOS.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 00466b80c1ab94f5984641b34a0a00f97e764773
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43464183"
---
# <a name="macoscredentialsinglesignonextension-resource-type"></a>tipo de recurso macOSCredentialSingleSignOnExtension

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um perfil de extensão de logon único de tipo de credencial para dispositivos macOS.


Herda de [macOSSingleSignOnExtension](../resources/intune-deviceconfig-macossinglesignonextension.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|extensionIdentifier|String|Obtém ou define a ID do pacote da extensão do aplicativo que executa o SSO para as URLs especificadas.|
|teamIdentifier|String|Obtém ou define a ID de equipe da extensão de aplicativo que executa o SSO para as URLs especificadas.|
|domínio|Coleção de cadeias de caracteres|Obtém ou define uma lista de hosts ou nomes de domínio para os quais a extensão de aplicativo executa SSO.|
|esfera|String|Obtém ou define o nome de território que diferencia maiúsculas de minúsculas para esse perfil.|
|as|coleção [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)|Obtém ou define uma lista de pares de valores de chave digitados usados para configurar perfis de tipo de credencial. Esta coleção pode conter um máximo de 500 elementos.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSCredentialSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSCredentialSingleSignOnExtension",
  "extensionIdentifier": "String",
  "teamIdentifier": "String",
  "domains": [
    "String"
  ],
  "realm": "String",
  "configurations": [
    {
      "@odata.type": "microsoft.graph.keyStringValuePair",
      "key": "String",
      "value": "String"
    }
  ]
}
```



