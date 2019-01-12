---
title: Membros
description: 'Descreve a visibilidade de uma equipe. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: b469a4db4bf535eaa4a7c6300a393381c92158fc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986436"
---
# <a name="teamvisibilitytype-enum-type"></a><span data-ttu-id="7da33-103">tipo de enum teamVisibilityType</span><span class="sxs-lookup"><span data-stu-id="7da33-103">teamVisibilityType enum type</span></span>

> <span data-ttu-id="7da33-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7da33-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7da33-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7da33-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7da33-106">Descreve a visibilidade de uma [equipe](../resources/team.md).</span><span class="sxs-lookup"><span data-stu-id="7da33-106">Describes the visibility of a [team](../resources/team.md).</span></span> 

## <a name="members"></a><span data-ttu-id="7da33-107">Membros</span><span class="sxs-lookup"><span data-stu-id="7da33-107">Members</span></span>

| <span data-ttu-id="7da33-108">Membro</span><span class="sxs-lookup"><span data-stu-id="7da33-108">Member</span></span> | <span data-ttu-id="7da33-109">Valor</span><span class="sxs-lookup"><span data-stu-id="7da33-109">Value</span></span>| <span data-ttu-id="7da33-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7da33-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="7da33-111">privada</span><span class="sxs-lookup"><span data-stu-id="7da33-111">private</span></span>|<span data-ttu-id="7da33-112">0</span><span class="sxs-lookup"><span data-stu-id="7da33-112">0</span></span>|<span data-ttu-id="7da33-113">Qualquer pessoa pode ver a equipe, mas apenas o proprietário pode adicionar um usuário para a equipe.</span><span class="sxs-lookup"><span data-stu-id="7da33-113">Anyone can see the team but only the owner can add a user to the team.</span></span>|
|<span data-ttu-id="7da33-114">public</span><span class="sxs-lookup"><span data-stu-id="7da33-114">public</span></span>|<span data-ttu-id="7da33-115">1</span><span class="sxs-lookup"><span data-stu-id="7da33-115">1</span></span>|<span data-ttu-id="7da33-116">Qualquer pessoa pode participar da equipe.</span><span class="sxs-lookup"><span data-stu-id="7da33-116">Anyone can join the team.</span></span>|
