---
title: Tipo de número de enrollmentState
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d208f8a4d1097d6698be3175a0b5ae86cf1918d4
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866794"
---
# <a name="enrollmentstate-enum-type"></a><span data-ttu-id="e08e7-103">Tipo de número de enrollmentState</span><span class="sxs-lookup"><span data-stu-id="e08e7-103">enrollmentState enum type</span></span>

<span data-ttu-id="e08e7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e08e7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e08e7-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e08e7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e08e7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e08e7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e08e7-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e08e7-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="e08e7-108">Membros</span><span class="sxs-lookup"><span data-stu-id="e08e7-108">Members</span></span>
|<span data-ttu-id="e08e7-109">Membro</span><span class="sxs-lookup"><span data-stu-id="e08e7-109">Member</span></span>|<span data-ttu-id="e08e7-110">Valor</span><span class="sxs-lookup"><span data-stu-id="e08e7-110">Value</span></span>|<span data-ttu-id="e08e7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e08e7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e08e7-112">desconhecido</span><span class="sxs-lookup"><span data-stu-id="e08e7-112">unknown</span></span>|<span data-ttu-id="e08e7-113">0</span><span class="sxs-lookup"><span data-stu-id="e08e7-113">0</span></span>|<span data-ttu-id="e08e7-114">O estado de registro do dispositivo é desconhecido</span><span class="sxs-lookup"><span data-stu-id="e08e7-114">Device enrollment state is unknown</span></span>|
|<span data-ttu-id="e08e7-115">inscrito</span><span class="sxs-lookup"><span data-stu-id="e08e7-115">enrolled</span></span>|<span data-ttu-id="e08e7-116">1</span><span class="sxs-lookup"><span data-stu-id="e08e7-116">1</span></span>|<span data-ttu-id="e08e7-117">O dispositivo está inscrito.</span><span class="sxs-lookup"><span data-stu-id="e08e7-117">Device is Enrolled.</span></span>|
|<span data-ttu-id="e08e7-118">pendingReset</span><span class="sxs-lookup"><span data-stu-id="e08e7-118">pendingReset</span></span>|<span data-ttu-id="e08e7-119">2</span><span class="sxs-lookup"><span data-stu-id="e08e7-119">2</span></span>|<span data-ttu-id="e08e7-120">Inscrito, mas ele é inscrito por meio do perfil de registro e o perfil inscrito é diferente do perfil atribuído.</span><span class="sxs-lookup"><span data-stu-id="e08e7-120">Enrolled but it's enrolled via enrollment profile and the enrolled profile is different from the assigned profile.</span></span>|
|<span data-ttu-id="e08e7-121">failed</span><span class="sxs-lookup"><span data-stu-id="e08e7-121">failed</span></span>|<span data-ttu-id="e08e7-122">3</span><span class="sxs-lookup"><span data-stu-id="e08e7-122">3</span></span>|<span data-ttu-id="e08e7-123">Não registrado e há registro de falha no registro.</span><span class="sxs-lookup"><span data-stu-id="e08e7-123">Not enrolled and there is enrollment failure record.</span></span>|
|<span data-ttu-id="e08e7-124">notContacted</span><span class="sxs-lookup"><span data-stu-id="e08e7-124">notContacted</span></span>|<span data-ttu-id="e08e7-125">4 </span><span class="sxs-lookup"><span data-stu-id="e08e7-125">4</span></span>|<span data-ttu-id="e08e7-126">O dispositivo é importado, mas não está inscrito.</span><span class="sxs-lookup"><span data-stu-id="e08e7-126">Device is imported but not enrolled.</span></span>|
|<span data-ttu-id="e08e7-127">blocked</span><span class="sxs-lookup"><span data-stu-id="e08e7-127">blocked</span></span>|<span data-ttu-id="e08e7-128">5 </span><span class="sxs-lookup"><span data-stu-id="e08e7-128">5</span></span>|<span data-ttu-id="e08e7-129">O dispositivo está inscrito como sem usuário, mas está impedido de mudar para o registro do usuário porque o aplicativo falhou na instalação.</span><span class="sxs-lookup"><span data-stu-id="e08e7-129">Device is enrolled as userless, but is blocked from moving to user enrollment because the app failed to install.</span></span>|




