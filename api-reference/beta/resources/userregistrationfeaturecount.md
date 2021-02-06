---
title: Tipo de recurso userRegistrationFeatureCount
description: Número de usuários registrados ou com capacidade para Autenticação Multifa factor, Self-Service redefinição de senha e autenticação sem senha.
author: danielwood95
localization_priority: Normal
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 7c73d9cd17d5bf13eb5f8899e0d1e9dc6e27af67
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132941"
---
# <a name="userregistrationfeaturecount-resource-type"></a>Tipo de recurso userRegistrationFeatureCount

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o número de usuários registrados ou com capacidade para Autenticação Multifa factor, Self-Service redefinição de senha e autenticação sem senha.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|recurso|authenticationMethodFeature|Número de usuários registrados ou com capacidade para Autenticação Multifa factor, Self-Service redefinição de senha e autenticação sem senha. Os valores possíveis são: `ssprRegistered`, `ssprEnabled`, `ssprCapable`, `passwordlessCapable`, `mfaCapable`.|
|userCount|Int64|Número de usuários.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userRegistrationFeatureCount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userRegistrationFeatureCount",
  "feature": "String",
  "userCount": "Integer"
}
```
