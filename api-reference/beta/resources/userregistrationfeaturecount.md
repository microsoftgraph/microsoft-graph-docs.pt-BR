---
title: Tipo de recurso userRegistrationFeatureCount
description: Número de usuários registrados ou capazes de autenticação multifator, Self-Service redefinição de senha e autenticação sem senha.
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 609c8d30547093c19d93428a0c779687b93ae018
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820159"
---
# <a name="userregistrationfeaturecount-resource-type"></a>Tipo de recurso userRegistrationFeatureCount

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o número de usuários registrados ou capazes de autenticação multifator, Self-Service redefinição de senha e autenticação sem senha.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|Recurso|authenticationMethodFeature|Número de usuários registrados ou capazes de autenticação multifator, Self-Service redefinição de senha e autenticação sem senha. Os valores possíveis são: `ssprRegistered`, `ssprEnabled`, `ssprCapable`, `passwordlessCapable`, `mfaCapable`.|
|userCount|Int64|Número de usuários|

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
