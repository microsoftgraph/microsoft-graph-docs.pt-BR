---
title: Tipo de recurso suggestedEnrollmentLimit
description: O recurso suggestedEnrollmentLimit representa o limite de inscrição sugerido quando dado um tipo de registro.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fca3ed6ad1d885fd01bc1aa313253a46b9acb4d7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59054335"
---
# <a name="suggestedenrollmentlimit-resource-type"></a>Tipo de recurso suggestedEnrollmentLimit

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O recurso suggestedEnrollmentLimit representa o limite de inscrição sugerido quando dado um tipo de registro.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|suggestedDailyLimit|Int32|O limite de inscrição sugerido dentro de um dia|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.suggestedEnrollmentLimit"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.suggestedEnrollmentLimit",
  "suggestedDailyLimit": 1024
}
```



