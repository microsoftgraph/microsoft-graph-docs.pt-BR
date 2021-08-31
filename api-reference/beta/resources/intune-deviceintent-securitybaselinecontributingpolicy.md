---
title: Tipo de recurso securityBaselineContributingPolicy
description: O estado de conformidade da linha de base de segurança de uma configuração para um dispositivo
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 92f49ce93e49524c3a9925e561cae57ca1c49f3d
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58803788"
---
# <a name="securitybaselinecontributingpolicy-resource-type"></a>Tipo de recurso securityBaselineContributingPolicy

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O estado de conformidade da linha de base de segurança de uma configuração para um dispositivo

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|sourceId|Cadeia de caracteres|Identificador exclusivo da política|
|displayName|Cadeia de caracteres|Nome da política|
|sourceType|[securityBaselinePolicySourceType](../resources/intune-deviceintent-securitybaselinepolicysourcetype.md)|Fonte de autoria da política. Os valores possíveis são: `deviceConfiguration`, `deviceIntent`.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.securityBaselineContributingPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineContributingPolicy",
  "sourceId": "String",
  "displayName": "String",
  "sourceType": "String"
}
```



