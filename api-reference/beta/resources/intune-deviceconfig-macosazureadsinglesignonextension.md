---
title: Tipo de recurso macOSAzureAdSingleSignOnExtension
description: Representa um perfil de extensão único do tipo Azure AD Sign-On para dispositivos macOS.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b7e4748b87a475b4f0ee7614054580926b502aeb
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59027096"
---
# <a name="macosazureadsinglesignonextension-resource-type"></a>Tipo de recurso macOSAzureAdSingleSignOnExtension

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um perfil de extensão único do tipo Azure AD Sign-On para dispositivos macOS.


Herda de [macOSSingleSignOnExtension](../resources/intune-deviceconfig-macossinglesignonextension.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|enableSharedDeviceMode|Booliano|Habilita ou desabilita o modo de dispositivo compartilhado.|
|bundleIdAccessControlList|String collection|Uma lista opcional de IDs de pacote adicionais permitidas para usar a extensão do AAD para um único login.|
|configurações|[Coleção keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)|Obtém ou define uma lista de pares de valores de chave digitados usados para configurar perfis de tipo de credencial. Esta coleção pode conter um máximo de 500 elementos.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSAzureAdSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSAzureAdSingleSignOnExtension",
  "enableSharedDeviceMode": true,
  "bundleIdAccessControlList": [
    "String"
  ],
  "configurations": [
    {
      "@odata.type": "microsoft.graph.keyStringValuePair",
      "key": "String",
      "value": "String"
    }
  ]
}
```



