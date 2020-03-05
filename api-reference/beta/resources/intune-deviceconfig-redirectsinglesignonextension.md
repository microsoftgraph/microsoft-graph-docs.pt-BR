---
title: tipo de recurso redirectSingleSignOnExtension
description: Representa uma extensão de logon único da Apple.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8398bcc1f10c91750b71928472290ccde55dad23
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529457"
---
# <a name="redirectsinglesignonextension-resource-type"></a>tipo de recurso redirectSingleSignOnExtension

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa uma extensão de logon único da Apple.


Herda de [singleSignOnExtension](../resources/intune-deviceconfig-singlesignonextension.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|extensionIdentifier|String|Obtém ou define a ID do pacote da extensão do aplicativo que executa o SSO para as URLs especificadas.|
|teamIdentifier|String|Obtém ou define a ID de equipe da extensão de aplicativo que executa o SSO para as URLs especificadas.|
|as|coleção [keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)|Obtém ou define uma lista de pares de valores de chave digitados usados para configurar perfis de tipo de credencial. Esta coleção pode conter um máximo de 500 elementos.|
|urlPrefixes|String collection|Um ou mais prefixos de URL de provedores de identidade em cujo nome a extensão do aplicativo executa logon único. As URLs devem começar com http://ou https://. Todos os prefixos de URL devem ser exclusivos para todos os perfis.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.redirectSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.redirectSingleSignOnExtension",
  "extensionIdentifier": "String",
  "teamIdentifier": "String",
  "configurations": [
    {
      "@odata.type": "microsoft.graph.keyStringValuePair",
      "key": "String",
      "value": "String"
    }
  ],
  "urlPrefixes": [
    "String"
  ]
}
```



