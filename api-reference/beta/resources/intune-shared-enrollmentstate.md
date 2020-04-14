---
title: tipo de enumeração de enrollmentid
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 5d4c3fa42d20bcf0540c55975d24aad596c8aebf
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43407753"
---
# <a name="enrollmentstate-enum-type"></a><span data-ttu-id="020f1-103">tipo de enumeração de enrollmentid</span><span class="sxs-lookup"><span data-stu-id="020f1-103">enrollmentState enum type</span></span>

<span data-ttu-id="020f1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="020f1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="020f1-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="020f1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="020f1-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="020f1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="020f1-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="020f1-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="020f1-108">Membros</span><span class="sxs-lookup"><span data-stu-id="020f1-108">Members</span></span>
|<span data-ttu-id="020f1-109">Membro</span><span class="sxs-lookup"><span data-stu-id="020f1-109">Member</span></span>|<span data-ttu-id="020f1-110">Valor</span><span class="sxs-lookup"><span data-stu-id="020f1-110">Value</span></span>|<span data-ttu-id="020f1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="020f1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="020f1-112">desconhecido</span><span class="sxs-lookup"><span data-stu-id="020f1-112">unknown</span></span>|<span data-ttu-id="020f1-113">,0</span><span class="sxs-lookup"><span data-stu-id="020f1-113">0</span></span>|<span data-ttu-id="020f1-114">O estado do registro do dispositivo é desconhecido</span><span class="sxs-lookup"><span data-stu-id="020f1-114">Device enrollment state is unknown</span></span>|
|<span data-ttu-id="020f1-115">registrados</span><span class="sxs-lookup"><span data-stu-id="020f1-115">enrolled</span></span>|<span data-ttu-id="020f1-116">1</span><span class="sxs-lookup"><span data-stu-id="020f1-116">1</span></span>|<span data-ttu-id="020f1-117">O dispositivo está inscrito.</span><span class="sxs-lookup"><span data-stu-id="020f1-117">Device is Enrolled.</span></span>|
|<span data-ttu-id="020f1-118">pendingReset</span><span class="sxs-lookup"><span data-stu-id="020f1-118">pendingReset</span></span>|<span data-ttu-id="020f1-119">duas</span><span class="sxs-lookup"><span data-stu-id="020f1-119">2</span></span>|<span data-ttu-id="020f1-120">Inscrito, mas ele está inscrito via perfil de registro e o perfil inscrito é diferente do perfil atribuído.</span><span class="sxs-lookup"><span data-stu-id="020f1-120">Enrolled but it's enrolled via enrollment profile and the enrolled profile is different from the assigned profile.</span></span>|
|<span data-ttu-id="020f1-121">falhou</span><span class="sxs-lookup"><span data-stu-id="020f1-121">failed</span></span>|<span data-ttu-id="020f1-122">3D</span><span class="sxs-lookup"><span data-stu-id="020f1-122">3</span></span>|<span data-ttu-id="020f1-123">Não registrado e o registro de falha de registro.</span><span class="sxs-lookup"><span data-stu-id="020f1-123">Not enrolled and there is enrollment failure record.</span></span>|
|<span data-ttu-id="020f1-124">Não contatado</span><span class="sxs-lookup"><span data-stu-id="020f1-124">notContacted</span></span>|<span data-ttu-id="020f1-125">4 </span><span class="sxs-lookup"><span data-stu-id="020f1-125">4</span></span>|<span data-ttu-id="020f1-126">O dispositivo é importado, mas não está inscrito.</span><span class="sxs-lookup"><span data-stu-id="020f1-126">Device is imported but not enrolled.</span></span>|
|<span data-ttu-id="020f1-127">bloqueou</span><span class="sxs-lookup"><span data-stu-id="020f1-127">blocked</span></span>|<span data-ttu-id="020f1-128">5 </span><span class="sxs-lookup"><span data-stu-id="020f1-128">5</span></span>|<span data-ttu-id="020f1-129">O dispositivo está inscrito como um não-usuário, mas é impedido de migrar para o registro do usuário porque o aplicativo não pôde ser instalado.</span><span class="sxs-lookup"><span data-stu-id="020f1-129">Device is enrolled as userless, but is blocked from moving to user enrollment because the app failed to install.</span></span>|



