---
title: Tipo de recurso macOSRedirectSingleSignOnExtension
description: Representa um perfil de extensão single Sign-On tipo de redirecionamento para dispositivos macOS.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: de39c91ddfc611d31e89837f6d894734eb031502
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59047125"
---
# <a name="macosredirectsinglesignonextension-resource-type"></a>Tipo de recurso macOSRedirectSingleSignOnExtension

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um perfil de extensão single Sign-On tipo de redirecionamento para dispositivos macOS.


Herda de [macOSSingleSignOnExtension](../resources/intune-deviceconfig-macossinglesignonextension.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|extensionIdentifier|Cadeia de Caracteres|Obtém ou define a ID do pacote da extensão do aplicativo que executa o SSO para as URLs especificadas.|
|teamIdentifier|Cadeia de Caracteres|Obtém ou define a ID de equipe da extensão do aplicativo que executa o SSO para as URLs especificadas.|
|configurações|[Coleção keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)|Obtém ou define uma lista de pares de valores de chave digitados usados para configurar perfis de tipo de credencial. Esta coleção pode conter um máximo de 500 elementos.|
|urlPrefixes|Conjunto de cadeias de caracteres|Um ou mais prefixos de URL de provedores de identidade em cujo nome a extensão do aplicativo realiza um único login. AS URLs devem começar com http:// ou https://. Todos os prefixos de URL devem ser exclusivos para todos os perfis.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSRedirectSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSRedirectSingleSignOnExtension",
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



