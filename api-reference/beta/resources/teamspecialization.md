---
title: tipo de enum teamSpecialization
description: Descreve o caso de uso especial para uma equipe.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 02a2272ee085d0c265adc9ce2e3f1c598e45be21
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930282"
---
# <a name="teamspecialization-enum-type"></a><span data-ttu-id="b381c-103">tipo de enum teamSpecialization</span><span class="sxs-lookup"><span data-stu-id="b381c-103">teamSpecialization enum type</span></span>

> <span data-ttu-id="b381c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b381c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b381c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b381c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b381c-106">Indica se a [equipe](../resources/team.md) destina-se de um caso de uso específico.</span><span class="sxs-lookup"><span data-stu-id="b381c-106">Indicates whether the [team](../resources/team.md) is intended for a particular use case.</span></span> <span data-ttu-id="b381c-107">Especialização cada [equipe](../resources/team.md) tem acesso aos comportamentos exclusivos e experiências destinadas ao seu caso de uso.</span><span class="sxs-lookup"><span data-stu-id="b381c-107">Each [team](../resources/team.md) specialization has access to unique behaviors and experiences targeted to its use case.</span></span> <span data-ttu-id="b381c-108">O padrão é 'Nenhum'.</span><span class="sxs-lookup"><span data-stu-id="b381c-108">Default is 'none'.</span></span>

## <a name="members"></a><span data-ttu-id="b381c-109">Membros</span><span class="sxs-lookup"><span data-stu-id="b381c-109">Members</span></span>

| <span data-ttu-id="b381c-110">Membro</span><span class="sxs-lookup"><span data-stu-id="b381c-110">Member</span></span>             | <span data-ttu-id="b381c-111">Valor</span><span class="sxs-lookup"><span data-stu-id="b381c-111">Value</span></span> | <span data-ttu-id="b381c-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b381c-112">Description</span></span>                                                                |
| :----------------- | :---- | :------------------------------------------------------------------------- |
| <span data-ttu-id="b381c-113">nenhum</span><span class="sxs-lookup"><span data-stu-id="b381c-113">none</span></span>               | <span data-ttu-id="b381c-114">0</span><span class="sxs-lookup"><span data-stu-id="b381c-114">0</span></span>     | <span data-ttu-id="b381c-115">Tipo de uma equipe que dá a experiência de equipe padrão padrão.</span><span class="sxs-lookup"><span data-stu-id="b381c-115">Default type for a team which gives the standard team experience.</span></span>          |
| <span data-ttu-id="b381c-116">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="b381c-116">unknownFutureValue</span></span> | <span data-ttu-id="b381c-117">7</span><span class="sxs-lookup"><span data-stu-id="b381c-117">7</span></span>     | <span data-ttu-id="b381c-118">Sentinel valor reservado como um espaço reservado para expansão futura do enum.</span><span class="sxs-lookup"><span data-stu-id="b381c-118">Sentinel value reserved as a placeholder for future expansion of the enum.</span></span> |
