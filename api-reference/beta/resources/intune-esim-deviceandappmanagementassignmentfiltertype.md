---
title: tipo de enumeração deviceAndAppManagementAssignmentFilterType
description: Representa o tipo do filtro de atribuição.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4e1febcc506de1248f519be5cd1c2d40fca9dc15
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43358099"
---
# <a name="deviceandappmanagementassignmentfiltertype-enum-type"></a><span data-ttu-id="66e8a-103">tipo de enumeração deviceAndAppManagementAssignmentFilterType</span><span class="sxs-lookup"><span data-stu-id="66e8a-103">deviceAndAppManagementAssignmentFilterType enum type</span></span>

<span data-ttu-id="66e8a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66e8a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="66e8a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="66e8a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66e8a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="66e8a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66e8a-107">Representa o tipo do filtro de atribuição.</span><span class="sxs-lookup"><span data-stu-id="66e8a-107">Represents type of the assignment filter.</span></span>

## <a name="members"></a><span data-ttu-id="66e8a-108">Membros</span><span class="sxs-lookup"><span data-stu-id="66e8a-108">Members</span></span>
|<span data-ttu-id="66e8a-109">Membro</span><span class="sxs-lookup"><span data-stu-id="66e8a-109">Member</span></span>|<span data-ttu-id="66e8a-110">Valor</span><span class="sxs-lookup"><span data-stu-id="66e8a-110">Value</span></span>|<span data-ttu-id="66e8a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="66e8a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66e8a-112">nenhuma</span><span class="sxs-lookup"><span data-stu-id="66e8a-112">none</span></span>|<span data-ttu-id="66e8a-113">,0</span><span class="sxs-lookup"><span data-stu-id="66e8a-113">0</span></span>|<span data-ttu-id="66e8a-114">Valor padrão.</span><span class="sxs-lookup"><span data-stu-id="66e8a-114">Default value.</span></span> <span data-ttu-id="66e8a-115">Não usar.</span><span class="sxs-lookup"><span data-stu-id="66e8a-115">Do not use.</span></span>|
|<span data-ttu-id="66e8a-116">ser</span><span class="sxs-lookup"><span data-stu-id="66e8a-116">include</span></span>|<span data-ttu-id="66e8a-117">1</span><span class="sxs-lookup"><span data-stu-id="66e8a-117">1</span></span>|<span data-ttu-id="66e8a-118">Indica em-Filter, a correspondência de regra oferecerá a carga aos dispositivos.</span><span class="sxs-lookup"><span data-stu-id="66e8a-118">Indicates in-filter, rule matching will offer the payload to devices.</span></span>|
|<span data-ttu-id="66e8a-119">impedir</span><span class="sxs-lookup"><span data-stu-id="66e8a-119">exclude</span></span>|<span data-ttu-id="66e8a-120">duas</span><span class="sxs-lookup"><span data-stu-id="66e8a-120">2</span></span>|<span data-ttu-id="66e8a-121">Indica ausência temporária, a correspondência de regra não oferecerá a carga aos dispositivos.</span><span class="sxs-lookup"><span data-stu-id="66e8a-121">Indicates out-filter, rule matching will not offer the payload to devices.</span></span>|



