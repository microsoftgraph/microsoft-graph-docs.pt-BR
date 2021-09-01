---
title: Tipo de recurso credentialSingleSignOnExtension
description: Representa um perfil de extensão Single Sign-On tipo de credencial.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 49c482d4c2c7027559a80cb2f4f55990d4f95b29
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58786015"
---
# <a name="credentialsinglesignonextension-resource-type"></a>Tipo de recurso credentialSingleSignOnExtension

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa um perfil de extensão Single Sign-On tipo de credencial.


Herda [de singleSignOnExtension](../resources/intune-deviceconfig-singlesignonextension.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|extensionIdentifier|Cadeia de caracteres|Obtém ou define a ID do pacote da extensão do aplicativo que executa o SSO para as URLs especificadas.|
|teamIdentifier|Cadeia de caracteres|Obtém ou define a ID de equipe da extensão do aplicativo que executa o SSO para as URLs especificadas.|
|domínios|Coleção de cadeias de caracteres|Obtém ou define uma lista de hosts ou nomes de domínio para os quais a extensão do aplicativo executa SSO.|
|realm|Cadeia de caracteres|Obtém ou define o nome do realm que diferencia minúsculas para esse perfil.|
|configurações|[Coleção keyTypedValuePair](../resources/intune-deviceconfig-keytypedvaluepair.md)|Obtém ou define uma lista de pares de valores de chave digitados usados para configurar perfis de tipo de credencial. Esta coleção pode conter um máximo de 500 elementos.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.credentialSingleSignOnExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.credentialSingleSignOnExtension",
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



