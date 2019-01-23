---
title: tipo de enum enrollmentState
description: Ainda não documentado
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b71f41d459e3fdb50fd853c62a855b4591a8ca8e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419104"
---
# <a name="enrollmentstate-enum-type"></a><span data-ttu-id="e221f-103">tipo de enum enrollmentState</span><span class="sxs-lookup"><span data-stu-id="e221f-103">enrollmentState enum type</span></span>

> <span data-ttu-id="e221f-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="e221f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e221f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e221f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e221f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="e221f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e221f-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e221f-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="e221f-108">Membros</span><span class="sxs-lookup"><span data-stu-id="e221f-108">Members</span></span>
|<span data-ttu-id="e221f-109">Membro</span><span class="sxs-lookup"><span data-stu-id="e221f-109">Member</span></span>|<span data-ttu-id="e221f-110">Valor</span><span class="sxs-lookup"><span data-stu-id="e221f-110">Value</span></span>|<span data-ttu-id="e221f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e221f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e221f-112">unknown</span><span class="sxs-lookup"><span data-stu-id="e221f-112">unknown</span></span>|<span data-ttu-id="e221f-113">0</span><span class="sxs-lookup"><span data-stu-id="e221f-113">0</span></span>|<span data-ttu-id="e221f-114">O estado de inscrição do dispositivo é desconhecido</span><span class="sxs-lookup"><span data-stu-id="e221f-114">Device enrollment state is unknown</span></span>|
|<span data-ttu-id="e221f-115">inscritos</span><span class="sxs-lookup"><span data-stu-id="e221f-115">enrolled</span></span>|<span data-ttu-id="e221f-116">1</span><span class="sxs-lookup"><span data-stu-id="e221f-116">1</span></span>|<span data-ttu-id="e221f-117">Inscrever-se o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e221f-117">Device is Enrolled.</span></span>|
|<span data-ttu-id="e221f-118">pendingReset</span><span class="sxs-lookup"><span data-stu-id="e221f-118">pendingReset</span></span>|<span data-ttu-id="e221f-119">2</span><span class="sxs-lookup"><span data-stu-id="e221f-119">2</span></span>|<span data-ttu-id="e221f-120">Inscritos, mas ele está inscrito via perfil de inscrição e o perfil registrado é diferente do perfil atribuído.</span><span class="sxs-lookup"><span data-stu-id="e221f-120">Enrolled but it's enrolled via enrollment profile and the enrolled profile is different from the assigned profile.</span></span>|
|<span data-ttu-id="e221f-121">Falha</span><span class="sxs-lookup"><span data-stu-id="e221f-121">failed</span></span>|<span data-ttu-id="e221f-122">3</span><span class="sxs-lookup"><span data-stu-id="e221f-122">3</span></span>|<span data-ttu-id="e221f-123">Não inscritos e não houver registro de falha de inscrição.</span><span class="sxs-lookup"><span data-stu-id="e221f-123">Not enrolled and there is enrollment failure record.</span></span>|
|<span data-ttu-id="e221f-124">notContacted</span><span class="sxs-lookup"><span data-stu-id="e221f-124">notContacted</span></span>|<span data-ttu-id="e221f-125">4</span><span class="sxs-lookup"><span data-stu-id="e221f-125">4</span></span>|<span data-ttu-id="e221f-126">Dispositivo é importado, mas não inscritos.</span><span class="sxs-lookup"><span data-stu-id="e221f-126">Device is imported but not enrolled.</span></span>|
|<span data-ttu-id="e221f-127">bloqueado</span><span class="sxs-lookup"><span data-stu-id="e221f-127">blocked</span></span>|<span data-ttu-id="e221f-128">5</span><span class="sxs-lookup"><span data-stu-id="e221f-128">5</span></span>|<span data-ttu-id="e221f-129">Dispositivo está inscrito como userless, mas seja bloqueado para mover para a inscrição do usuário porque o aplicativo falha na instalação.</span><span class="sxs-lookup"><span data-stu-id="e221f-129">Device is enrolled as userless, but is blocked from moving to user enrollment because the app failed to install.</span></span>|




