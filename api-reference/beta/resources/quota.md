---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Cota
localization_priority: Normal
ms.openlocfilehash: a63b41253569dbb3d666a76b0a7495839ef61b12
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882408"
---
# <a name="quota-resource-type"></a>tipo de recurso de cota

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

O recurso de **cota** fornece detalhes sobre o espaço restringe em um recurso de [unidade](drive.md) .

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@odata.type": "microsoft.graph.quota"
}-->

```json
{
  "deleted": 1024,
  "remaining": 1024,
  "state": "normal | nearing | critical | exceeded",
  "storagePlanInformation": {
    "upgradeAvailable": true
  },
  "total": 1024,
  "used": 1024
}
```

## <a name="properties"></a>Propriedades

| Nome da propriedade | Tipo   | Descrição                                                                 |
|:--------------|:-------|:----------------------------------------------------------------------------|
| total         | Int64  | Espaço de armazenamento permitido total, em bytes. Somente leitura.                           |
| used          | Int64  | Espaço total, em bytes. Somente leitura.                                      |
| remaining     | Int64  | Espaço total restante antes de atingir o limite de cota, em bytes. Somente leitura. |
| deleted       | Int64  | Espaço total consumido por arquivos na Lixeira, em bytes. Somente leitura.      |
| estado         | string | Valor de enumeração que indica o estado do espaço de armazenamento. Somente leitura. |
| storagePlanInformation  | [storagePlanInformation](storageplaninformation.md) | Informações sobre planos de cota de armazenamento da unidade. Somente no OneDrive pessoal.|

### <a name="state-enumeration-values"></a>Valores de enumeração State

| Valor      | Descrição                                                                                                                                                                 |
|:-----------|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `normal`   | A unidade tem bastante cota restante.                                                                                                                               |
| `nearing`  | A cota restante é inferior a 10% do espaço de cota total.                                                                                                                      |
| `critical` | A cota restante é inferior a 1% do espaço de cota total.                                                                                                                       |
| `exceeded` | A cota usada excedeu a cota total. Novos arquivos ou pastas não podem ser adicionadas à unidade até que ela esteja abaixo da quantidade total de cotas ou mais espaço de armazenamento seja adquirido. |

<!-- {
  "type": "#page.annotation",
  "description": "The quota facet provides information about how much space the OneDrive has available.",
  "keywords": "quota,available,remaining,used",
  "section": "documentation",
  "tocPath": "Facets/Quota"
} -->
