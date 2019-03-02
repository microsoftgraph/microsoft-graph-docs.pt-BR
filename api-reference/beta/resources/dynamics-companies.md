---
title: tipo de recurso de empresas
description: Uma empresa no Dynamics 365 Business central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: f1faca36af25bc8cb3e9019e0dc5b4460991e70d
ms.sourcegitcommit: f2444a37a719b87777bdddbd086f106746fa0a1c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/02/2019
ms.locfileid: "30365679"
---
# <a name="companies-resource-type"></a>tipo de recurso de empresas
Representa um tipo de recurso de empresas no Dynamics 365 Business central. 

## <a name="methods"></a>Métodos

| Método         | Tipo de retorno  |Descrição|
|:---------------|:-------------|:----------|
|[Obter empresas](../api/dynamics-companies-get.md)|companhias|Obter uma empresa.|

## <a name="properties"></a>Propriedades
| Propriedade        | Tipo |Descrição                             |
|:----------------|:-----|:---------------------------------------|
|id               |GUID  |A identificação exclusiva da empresa. Somente Leitura.|
|name             |string|Especifica a empresa.                  |
|displayName      |string|Especifica o nome de exibição da empresa.     |
|systemVersion    |string|Especifica a versão interna da empresa.|
|businessProfileId|string|Especifica a ID do perfil de negócios vinculada à empresa.|


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON da empresa.

```json
{
  "id": "GUID",
  "name": "string",
  "displayName": "string",
  "systemVersion": "string",
  "businessProfileId": "string"
}

```


