---
title: Tipo de recurso excludeTarget
description: Representa os usuários ou grupos de usuários excluídos de uma política.
author: mjsantani
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9d2786a6107e524fe00430658542dea374cae275
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682868"
---
# <a name="excludetarget-resource-type"></a><span data-ttu-id="3bf18-103">Tipo de recurso excludeTarget</span><span class="sxs-lookup"><span data-stu-id="3bf18-103">excludeTarget resource type</span></span>

<span data-ttu-id="3bf18-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3bf18-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3bf18-105">Representa os usuários ou grupos de usuários excluídos de uma política.</span><span class="sxs-lookup"><span data-stu-id="3bf18-105">Represents the users or groups of users that are excluded from a policy.</span></span>

## <a name="properties"></a><span data-ttu-id="3bf18-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3bf18-106">Properties</span></span>
|<span data-ttu-id="3bf18-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3bf18-107">Property</span></span>|<span data-ttu-id="3bf18-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="3bf18-108">Type</span></span>|<span data-ttu-id="3bf18-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3bf18-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3bf18-110">id</span><span class="sxs-lookup"><span data-stu-id="3bf18-110">id</span></span>|<span data-ttu-id="3bf18-111">String</span><span class="sxs-lookup"><span data-stu-id="3bf18-111">String</span></span>|<span data-ttu-id="3bf18-112">O identificador de objeto de um usuário ou grupo do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="3bf18-112">The object identifier of an Azure AD user or group.</span></span>|
|<span data-ttu-id="3bf18-113">targetType</span><span class="sxs-lookup"><span data-stu-id="3bf18-113">targetType</span></span>|<span data-ttu-id="3bf18-114">authenticationMethodTargetType</span><span class="sxs-lookup"><span data-stu-id="3bf18-114">authenticationMethodTargetType</span></span>|<span data-ttu-id="3bf18-115">O tipo de destino do método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="3bf18-115">The type of the authentication method target.</span></span> <span data-ttu-id="3bf18-116">Os valores possíveis são: `user`, `group`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="3bf18-116">Possible values are: `user`, `group`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3bf18-117">Relações</span><span class="sxs-lookup"><span data-stu-id="3bf18-117">Relationships</span></span>
<span data-ttu-id="3bf18-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3bf18-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3bf18-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3bf18-119">JSON representation</span></span>
<span data-ttu-id="3bf18-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3bf18-120">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.excludeTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.excludeTarget",
  "id": "String (identifier)",
  "targetType": "String"
}
```
