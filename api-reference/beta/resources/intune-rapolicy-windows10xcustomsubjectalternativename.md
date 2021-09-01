---
title: Tipo de recurso windows10XCustomSubjectAlternativeName
description: Tipo de perfil base para certificados de autenticação (SCEP ou PFX Create)
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 842e6b171b5a82a163c6f9aa578ef9cbb869dc6b
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58796829"
---
# <a name="windows10xcustomsubjectalternativename-resource-type"></a>Tipo de recurso windows10XCustomSubjectAlternativeName

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Tipo de perfil base para certificados de autenticação (SCEP ou PFX Create)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|sanType|[subjectAlternativeNameType](../resources/intune-shared-subjectalternativenametype.md)|Tipo SAN personalizado. Os possíveis valores são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.|
|nome|Cadeia de caracteres|Nome SAN personalizado|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10XCustomSubjectAlternativeName"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10XCustomSubjectAlternativeName",
  "sanType": "String",
  "name": "String"
}
```



