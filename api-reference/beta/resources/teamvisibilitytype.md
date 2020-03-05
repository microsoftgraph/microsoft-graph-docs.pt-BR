---
title: Members
description: 'Descreve a visibilidade de uma equipe. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: enumPageType
ms.openlocfilehash: d0e043fa05b6f1f3717d8ec2d83d62f3ec3437fd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519803"
---
# <a name="teamvisibilitytype-enum-type"></a><span data-ttu-id="9c347-103">tipo de enumeração teamVisibilityType</span><span class="sxs-lookup"><span data-stu-id="9c347-103">teamVisibilityType enum type</span></span>

<span data-ttu-id="9c347-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="9c347-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c347-105">Descreve a visibilidade de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="9c347-105">Describes the visibility of a [team](../resources/team.md).</span></span> 

## <a name="members"></a><span data-ttu-id="9c347-106">Membros</span><span class="sxs-lookup"><span data-stu-id="9c347-106">Members</span></span>

| <span data-ttu-id="9c347-107">Membro</span><span class="sxs-lookup"><span data-stu-id="9c347-107">Member</span></span> | <span data-ttu-id="9c347-108">Valor</span><span class="sxs-lookup"><span data-stu-id="9c347-108">Value</span></span>| <span data-ttu-id="9c347-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c347-109">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="9c347-110">privada</span><span class="sxs-lookup"><span data-stu-id="9c347-110">private</span></span>|<span data-ttu-id="9c347-111">,0</span><span class="sxs-lookup"><span data-stu-id="9c347-111">0</span></span>|<span data-ttu-id="9c347-112">Qualquer pessoa pode ver a equipe, mas apenas o proprietário pode adicionar um usuário à equipe.</span><span class="sxs-lookup"><span data-stu-id="9c347-112">Anyone can see the team but only the owner can add a user to the team.</span></span>|
|<span data-ttu-id="9c347-113">public</span><span class="sxs-lookup"><span data-stu-id="9c347-113">public</span></span>|<span data-ttu-id="9c347-114">1 </span><span class="sxs-lookup"><span data-stu-id="9c347-114">1</span></span>|<span data-ttu-id="9c347-115">Qualquer pessoa pode participar da equipe.</span><span class="sxs-lookup"><span data-stu-id="9c347-115">Anyone can join the team.</span></span>|
