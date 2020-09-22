---
title: tipo de recurso suggestedEnrollmentLimit
description: O recurso suggestedEnrollmentLimit representa o limite de inscrição sugerido quando é atribuído um tipo de registro.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 99efb75bcf52b841dcf67741045b7207a85eb3cc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081957"
---
# <a name="suggestedenrollmentlimit-resource-type"></a>tipo de recurso suggestedEnrollmentLimit

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O recurso suggestedEnrollmentLimit representa o limite de inscrição sugerido quando é atribuído um tipo de registro.

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






