---
title: tipo de recurso windowsKioskAzureADGroup
description: A classe usada para identificar um grupo do AzureAD para a configuração do quiosque
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f05bf9d01e8442a54c9fa70b863e3789309bd9d4
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30175133"
---
# <a name="windowskioskazureadgroup-resource-type"></a>tipo de recurso windowsKioskAzureADGroup

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

A classe usada para identificar um grupo do AzureAD para a configuração do quiosque


Herda de [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|O nome de exibição do grupo AzureAD que será bloqueado para esta configuração de quiosque|
|groupId|String|A ID do grupo AzureAD que será bloqueado para esta configuração de quiosque|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAzureADGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAzureADGroup",
  "displayName": "String",
  "groupId": "String"
}
```




