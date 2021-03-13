---
title: tipo bitlocker
description: Recurso BitLocker
author: hafowler
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 3e714015b3834051371861880355360f02d12166
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761832"
---
# <a name="bitlocker-resource-type"></a><span data-ttu-id="03b9a-103">Tipo de recurso bitlocker</span><span class="sxs-lookup"><span data-stu-id="03b9a-103">bitlocker resource type</span></span>

<span data-ttu-id="03b9a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03b9a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03b9a-105">O recurso pai de uma chave BitLocker armazenada com a propriedade de navegação **bitlockerRecoveryKey** que contém a chave de recuperação real.</span><span class="sxs-lookup"><span data-stu-id="03b9a-105">The parent resource for a stored BitLocker key with the navigation property **bitlockerRecoveryKey** which contains the actual recovery key.</span></span>

## <a name="methods"></a><span data-ttu-id="03b9a-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="03b9a-106">Methods</span></span>
|<span data-ttu-id="03b9a-107">Método</span><span class="sxs-lookup"><span data-stu-id="03b9a-107">Method</span></span>|<span data-ttu-id="03b9a-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="03b9a-108">Return type</span></span>|<span data-ttu-id="03b9a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="03b9a-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="03b9a-110">Listar recoveryKeys</span><span class="sxs-lookup"><span data-stu-id="03b9a-110">List recoveryKeys</span></span>](../api/bitlocker-list-recoverykeys.md)|<span data-ttu-id="03b9a-111">[Coleção bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md)</span><span class="sxs-lookup"><span data-stu-id="03b9a-111">[bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) collection</span></span>|<span data-ttu-id="03b9a-112">Obter uma lista dos objetos bitlockerRecoveryKey e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="03b9a-112">Get a list of the bitlockerRecoveryKey objects and their properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="03b9a-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="03b9a-113">Properties</span></span>
<span data-ttu-id="03b9a-114">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="03b9a-114">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="03b9a-115">Relações</span><span class="sxs-lookup"><span data-stu-id="03b9a-115">Relationships</span></span>
| <span data-ttu-id="03b9a-116">Relação</span><span class="sxs-lookup"><span data-stu-id="03b9a-116">Relationship</span></span> | <span data-ttu-id="03b9a-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="03b9a-117">Type</span></span> | <span data-ttu-id="03b9a-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="03b9a-118">Description</span></span> |
|--|--|--|
| <span data-ttu-id="03b9a-119">recoveryKeys</span><span class="sxs-lookup"><span data-stu-id="03b9a-119">recoveryKeys</span></span> | <span data-ttu-id="03b9a-120">[Coleção bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md)</span><span class="sxs-lookup"><span data-stu-id="03b9a-120">[bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) collection</span></span> | <span data-ttu-id="03b9a-121">As chaves de recuperação associadas à entidade bitlocker.</span><span class="sxs-lookup"><span data-stu-id="03b9a-121">The recovery keys associated with the bitlocker entity.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="03b9a-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="03b9a-122">JSON representation</span></span>
<span data-ttu-id="03b9a-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="03b9a-123">The following is a JSON representation of the resource.</span></span>
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

