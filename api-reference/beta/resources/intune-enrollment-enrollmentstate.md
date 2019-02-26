---
title: tipo de enumeração de enrollmentid
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dcb039563d9c45a33c4e42344fc8557dfe29b333
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159245"
---
# <a name="enrollmentstate-enum-type"></a><span data-ttu-id="99a8b-103">tipo de enumeração de enrollmentid</span><span class="sxs-lookup"><span data-stu-id="99a8b-103">enrollmentState enum type</span></span>

> <span data-ttu-id="99a8b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="99a8b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99a8b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="99a8b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99a8b-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="99a8b-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="99a8b-107">Membros</span><span class="sxs-lookup"><span data-stu-id="99a8b-107">Members</span></span>
|<span data-ttu-id="99a8b-108">Membro</span><span class="sxs-lookup"><span data-stu-id="99a8b-108">Member</span></span>|<span data-ttu-id="99a8b-109">Valor</span><span class="sxs-lookup"><span data-stu-id="99a8b-109">Value</span></span>|<span data-ttu-id="99a8b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="99a8b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99a8b-111">unknown</span><span class="sxs-lookup"><span data-stu-id="99a8b-111">unknown</span></span>|<span data-ttu-id="99a8b-112">,0</span><span class="sxs-lookup"><span data-stu-id="99a8b-112">0</span></span>|<span data-ttu-id="99a8b-113">O estado do registro do dispositivo é desconhecido</span><span class="sxs-lookup"><span data-stu-id="99a8b-113">Device enrollment state is unknown</span></span>|
|<span data-ttu-id="99a8b-114">registrados</span><span class="sxs-lookup"><span data-stu-id="99a8b-114">enrolled</span></span>|<span data-ttu-id="99a8b-115">1</span><span class="sxs-lookup"><span data-stu-id="99a8b-115">1</span></span>|<span data-ttu-id="99a8b-116">O dispositivo está inscrito.</span><span class="sxs-lookup"><span data-stu-id="99a8b-116">Device is Enrolled.</span></span>|
|<span data-ttu-id="99a8b-117">pendingReset</span><span class="sxs-lookup"><span data-stu-id="99a8b-117">pendingReset</span></span>|<span data-ttu-id="99a8b-118">duas</span><span class="sxs-lookup"><span data-stu-id="99a8b-118">2</span></span>|<span data-ttu-id="99a8b-119">Inscrito, mas ele está inscrito via perfil de registro e o perfil inscrito é diferente do perfil atribuído.</span><span class="sxs-lookup"><span data-stu-id="99a8b-119">Enrolled but it's enrolled via enrollment profile and the enrolled profile is different from the assigned profile.</span></span>|
|<span data-ttu-id="99a8b-120">falhou</span><span class="sxs-lookup"><span data-stu-id="99a8b-120">failed</span></span>|<span data-ttu-id="99a8b-121">3D</span><span class="sxs-lookup"><span data-stu-id="99a8b-121">3</span></span>|<span data-ttu-id="99a8b-122">Não registrado e o registro de falha de registro.</span><span class="sxs-lookup"><span data-stu-id="99a8b-122">Not enrolled and there is enrollment failure record.</span></span>|
|<span data-ttu-id="99a8b-123">Não contatado</span><span class="sxs-lookup"><span data-stu-id="99a8b-123">notContacted</span></span>|<span data-ttu-id="99a8b-124">quatro</span><span class="sxs-lookup"><span data-stu-id="99a8b-124">4</span></span>|<span data-ttu-id="99a8b-125">O dispositivo é importado, mas não está inscrito.</span><span class="sxs-lookup"><span data-stu-id="99a8b-125">Device is imported but not enrolled.</span></span>|
|<span data-ttu-id="99a8b-126">bloqueou</span><span class="sxs-lookup"><span data-stu-id="99a8b-126">blocked</span></span>|<span data-ttu-id="99a8b-127">0,5</span><span class="sxs-lookup"><span data-stu-id="99a8b-127">5</span></span>|<span data-ttu-id="99a8b-128">O dispositivo está inscrito como um não-usuário, mas é impedido de migrar para o registro do usuário porque o aplicativo não pôde ser instalado.</span><span class="sxs-lookup"><span data-stu-id="99a8b-128">Device is enrolled as userless, but is blocked from moving to user enrollment because the app failed to install.</span></span>|




