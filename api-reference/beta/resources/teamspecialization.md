---
title: tipo de enumeração Teamsspecialization
description: Descreve o caso de uso especial de uma equipe.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: enumPageType
ms.openlocfilehash: 4d9705118fac4a72926ffeabe63c4b460e164002
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046458"
---
# <a name="teamspecialization-enum-type"></a><span data-ttu-id="8cfc7-103">tipo de enumeração Teamsspecialization</span><span class="sxs-lookup"><span data-stu-id="8cfc7-103">teamSpecialization enum type</span></span>

<span data-ttu-id="8cfc7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8cfc7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8cfc7-105">Indica se a [equipe](../resources/team.md) destina-se a um caso de uso específico.</span><span class="sxs-lookup"><span data-stu-id="8cfc7-105">Indicates whether the [team](../resources/team.md) is intended for a particular use case.</span></span> <span data-ttu-id="8cfc7-106">Cada especialização de [equipe](../resources/team.md) tem acesso a comportamentos e experiências exclusivos direcionados ao seu caso de uso.</span><span class="sxs-lookup"><span data-stu-id="8cfc7-106">Each [team](../resources/team.md) specialization has access to unique behaviors and experiences targeted to its use case.</span></span> <span data-ttu-id="8cfc7-107">O padrão é ' nenhum '.</span><span class="sxs-lookup"><span data-stu-id="8cfc7-107">Default is 'none'.</span></span>

## <a name="members"></a><span data-ttu-id="8cfc7-108">Membros</span><span class="sxs-lookup"><span data-stu-id="8cfc7-108">Members</span></span>

| <span data-ttu-id="8cfc7-109">Membro</span><span class="sxs-lookup"><span data-stu-id="8cfc7-109">Member</span></span>             | <span data-ttu-id="8cfc7-110">Valor</span><span class="sxs-lookup"><span data-stu-id="8cfc7-110">Value</span></span> | <span data-ttu-id="8cfc7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cfc7-111">Description</span></span>                                                                |
| :----------------- | :---- | :------------------------------------------------------------------------- |
| <span data-ttu-id="8cfc7-112">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="8cfc7-112">none</span></span>               | <span data-ttu-id="8cfc7-113">,0</span><span class="sxs-lookup"><span data-stu-id="8cfc7-113">0</span></span>     | <span data-ttu-id="8cfc7-114">O tipo padrão para uma equipe que oferece a experiência de equipe padrão.</span><span class="sxs-lookup"><span data-stu-id="8cfc7-114">Default type for a team which gives the standard team experience.</span></span>          |
| <span data-ttu-id="8cfc7-115">educationStandard</span><span class="sxs-lookup"><span data-stu-id="8cfc7-115">educationStandard</span></span>  | <span data-ttu-id="8cfc7-116">1 </span><span class="sxs-lookup"><span data-stu-id="8cfc7-116">1</span></span>     | <span data-ttu-id="8cfc7-117">Equipe criada por um usuário educacional.</span><span class="sxs-lookup"><span data-stu-id="8cfc7-117">Team created by an education user.</span></span> <span data-ttu-id="8cfc7-118">Todas as equipes criadas pelo usuário educacional são do tipo edu.</span><span class="sxs-lookup"><span data-stu-id="8cfc7-118">All teams created by education user are of type Edu.</span></span> |
| <span data-ttu-id="8cfc7-119">educationClass</span><span class="sxs-lookup"><span data-stu-id="8cfc7-119">educationClass</span></span>     | <span data-ttu-id="8cfc7-120">2 </span><span class="sxs-lookup"><span data-stu-id="8cfc7-120">2</span></span>     | <span data-ttu-id="8cfc7-121">Experiência de equipe otimizada para uma aula.</span><span class="sxs-lookup"><span data-stu-id="8cfc7-121">Team experience optimized for a class.</span></span> <span data-ttu-id="8cfc7-122">Isso habilita a segmentação de recursos no O365.</span><span class="sxs-lookup"><span data-stu-id="8cfc7-122">This enables segmentation of features across O365.</span></span> |
| <span data-ttu-id="8cfc7-123">educationProfessionalLearningCommunity</span><span class="sxs-lookup"><span data-stu-id="8cfc7-123">educationProfessionalLearningCommunity</span></span> | <span data-ttu-id="8cfc7-124">3 </span><span class="sxs-lookup"><span data-stu-id="8cfc7-124">3</span></span> | <span data-ttu-id="8cfc7-125">Experiência de equipe otimizada para um PLC.</span><span class="sxs-lookup"><span data-stu-id="8cfc7-125">Team experience optimized for a PLC.</span></span> <span data-ttu-id="8cfc7-126">Saiba mais sobre o PLC [aqui](https://en.wikipedia.org/wiki/Professional_learning_community).</span><span class="sxs-lookup"><span data-stu-id="8cfc7-126">Learn more about PLC [here](https://en.wikipedia.org/wiki/Professional_learning_community).</span></span> |
| <span data-ttu-id="8cfc7-127">educationStaff</span><span class="sxs-lookup"><span data-stu-id="8cfc7-127">educationStaff</span></span>     | <span data-ttu-id="8cfc7-128">4 </span><span class="sxs-lookup"><span data-stu-id="8cfc7-128">4</span></span>     |  <span data-ttu-id="8cfc7-129">Tipo de equipe para uma experiência otimizada para a equipe em uma organização, onde o líder da equipe, como o principal, é o administrador e os professores são membros de uma equipe que vem com um bloco de anotações especializado.</span><span class="sxs-lookup"><span data-stu-id="8cfc7-129">Team type for an optimized experience for staff in an organization, where a staff leader, like a principal, is the admin and teachers are members in a team that comes with a specialized notebook.</span></span> <span data-ttu-id="8cfc7-130">Para obter mais detalhes, consulte [bloco de anotações de equipe do OneNote para educação](https://www.onenote.com/staffnotebookedu).</span><span class="sxs-lookup"><span data-stu-id="8cfc7-130">For more details, see [OneNote staff notebook for education](https://www.onenote.com/staffnotebookedu).</span></span> |
| <span data-ttu-id="8cfc7-131">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="8cfc7-131">unknownFutureValue</span></span> | <span data-ttu-id="8cfc7-132">7 </span><span class="sxs-lookup"><span data-stu-id="8cfc7-132">7</span></span>     | <span data-ttu-id="8cfc7-133">O valor de sentinela reservado como um espaço reservado para expansão futura da enumeração.</span><span class="sxs-lookup"><span data-stu-id="8cfc7-133">Sentinel value reserved as a placeholder for future expansion of the enum.</span></span> |


