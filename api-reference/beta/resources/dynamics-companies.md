---
title: tipo de recurso de empresas
description: Uma empresa no Dynamics 365 Business Central.
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
ms.localizationpriority: medium
ms.prod: dynamics-365-business-central
doc_type: resourcePageType
ms.openlocfilehash: 8230e7aca8b222c54656845c0e52d4fc60bc7abd
ms.sourcegitcommit: 6b5bee1a1cea92c1f3d6439110c4916eb8b249a5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/11/2021
ms.locfileid: "60908570"
---
# <a name="companies-resource-type"></a>tipo de recurso de empresas

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um tipo de recurso de empresas no Dynamics 365 Business Central. 

## <a name="methods"></a>Métodos

| Método         | Tipo de retorno  |Descrição|
|:---------------|:-------------|:----------|
|[Obter empresas](../api/dynamics-companies-get.md)|companies|Obter uma empresa.|

## <a name="properties"></a>Propriedades
| Propriedade        | Tipo |Descrição                             |
|:----------------|:-----|:---------------------------------------|
|id               |GUID  |A ID exclusiva da empresa. Somente Leitura.|
|nome             |string|Especifica a Empresa.                  |
|displayName      |string|Especifica o nome de exibição da empresa.     |
|systemVersion    |string|Especifica a versão interna da empresa.|
|businessProfileId|string|Especifica a ID do Perfil de Negócios vinculada à empresa.|


## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON

Aqui está uma representação JSON da empresa.

```json
{
  "id": "GUID",
  "name": "string",
  "displayName": "string",
  "systemVersion": "string",
  "businessProfileId": "string"
}
```




