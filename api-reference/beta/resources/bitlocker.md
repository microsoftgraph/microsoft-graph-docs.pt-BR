---
title: tipo de BitLocker
description: Recurso do BitLocker
author: hafowler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3ad8a05e82cd3f300bedf034fe18f67ce3359f16
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48038862"
---
# <a name="bitlocker-resource-type"></a><span data-ttu-id="db830-103">tipo de recurso do BitLocker</span><span class="sxs-lookup"><span data-stu-id="db830-103">bitlocker resource type</span></span>

<span data-ttu-id="db830-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db830-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="db830-105">O recurso pai de uma chave do BitLocker armazenada com a propriedade de navegação **bitlockerRecoveryKey** que contém a chave de recuperação real.</span><span class="sxs-lookup"><span data-stu-id="db830-105">The parent resource for a stored BitLocker key with the navigation property **bitlockerRecoveryKey** which contains the actual recovery key.</span></span>

## <a name="methods"></a><span data-ttu-id="db830-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="db830-106">Methods</span></span>
|<span data-ttu-id="db830-107">Método</span><span class="sxs-lookup"><span data-stu-id="db830-107">Method</span></span>|<span data-ttu-id="db830-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="db830-108">Return type</span></span>|<span data-ttu-id="db830-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="db830-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="db830-110">Listar recoveryKeys</span><span class="sxs-lookup"><span data-stu-id="db830-110">List recoveryKeys</span></span>](../api/bitlocker-list-recoverykeys.md)|<span data-ttu-id="db830-111">coleção [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md)</span><span class="sxs-lookup"><span data-stu-id="db830-111">[bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) collection</span></span>|<span data-ttu-id="db830-112">Obtenha uma lista dos objetos bitlockerRecoveryKey e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="db830-112">Get a list of the bitlockerRecoveryKey objects and their properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="db830-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="db830-113">Properties</span></span>
<span data-ttu-id="db830-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="db830-114">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="db830-115">Relações</span><span class="sxs-lookup"><span data-stu-id="db830-115">Relationships</span></span>
| <span data-ttu-id="db830-116">Relação</span><span class="sxs-lookup"><span data-stu-id="db830-116">Relationship</span></span> | <span data-ttu-id="db830-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="db830-117">Type</span></span> | <span data-ttu-id="db830-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="db830-118">Description</span></span> |
|--|--|--|
| <span data-ttu-id="db830-119">recoveryKeys</span><span class="sxs-lookup"><span data-stu-id="db830-119">recoveryKeys</span></span> | <span data-ttu-id="db830-120">coleção [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md)</span><span class="sxs-lookup"><span data-stu-id="db830-120">[bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) collection</span></span> | <span data-ttu-id="db830-121">As chaves de recuperação associadas à entidade do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="db830-121">The recovery keys associated with the bitlocker entity.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="db830-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="db830-122">JSON representation</span></span>
<span data-ttu-id="db830-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="db830-123">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitlocker",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitlocker"
}
```

