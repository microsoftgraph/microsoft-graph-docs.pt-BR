---
title: Membros
description: 'Descreve a visibilidade de uma equipe. '
author: nkramer
ms.openlocfilehash: 5f03eb52a5eb7aa672998897e11fb5d3a358bf9a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305289"
---
# <a name="teamvisibilitytype-enum-type"></a><span data-ttu-id="a3b91-103">tipo de enum teamVisibilityType</span><span class="sxs-lookup"><span data-stu-id="a3b91-103">teamVisibilityType enum type</span></span>

> <span data-ttu-id="a3b91-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a3b91-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a3b91-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a3b91-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a3b91-106">Descreve a visibilidade de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="a3b91-106">Describes the visibility of a [team](../resources/team.md).</span></span> 

## <a name="members"></a><span data-ttu-id="a3b91-107">Membros</span><span class="sxs-lookup"><span data-stu-id="a3b91-107">Members</span></span>

| <span data-ttu-id="a3b91-108">Membro</span><span class="sxs-lookup"><span data-stu-id="a3b91-108">Member</span></span> | <span data-ttu-id="a3b91-109">Valor</span><span class="sxs-lookup"><span data-stu-id="a3b91-109">Value</span></span>| <span data-ttu-id="a3b91-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3b91-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="a3b91-111">privada</span><span class="sxs-lookup"><span data-stu-id="a3b91-111">private</span></span>|<span data-ttu-id="a3b91-112">0</span><span class="sxs-lookup"><span data-stu-id="a3b91-112">0</span></span>|<span data-ttu-id="a3b91-113">Qualquer pessoa pode ver a equipe, mas apenas o proprietário pode adicionar um usuário para a equipe.</span><span class="sxs-lookup"><span data-stu-id="a3b91-113">Anyone can see the team but only the owner can add a user to the team.</span></span>|
|<span data-ttu-id="a3b91-114">public</span><span class="sxs-lookup"><span data-stu-id="a3b91-114">public</span></span>|<span data-ttu-id="a3b91-115">1</span><span class="sxs-lookup"><span data-stu-id="a3b91-115">1</span></span>|<span data-ttu-id="a3b91-116">Qualquer pessoa pode participar da equipe.</span><span class="sxs-lookup"><span data-stu-id="a3b91-116">Anyone can join the team.</span></span>|
