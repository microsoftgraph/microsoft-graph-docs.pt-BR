---
title: tipo de enum enrollmentState
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9394755c5b6e6de8ed039b226d03074f1ef16cc3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933586"
---
# <a name="enrollmentstate-enum-type"></a><span data-ttu-id="b01c1-103">tipo de enum enrollmentState</span><span class="sxs-lookup"><span data-stu-id="b01c1-103">enrollmentState enum type</span></span>

> <span data-ttu-id="b01c1-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b01c1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b01c1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b01c1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b01c1-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b01c1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b01c1-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b01c1-107">Not yet documented</span></span>
## <a name="members"></a><span data-ttu-id="b01c1-108">Membros</span><span class="sxs-lookup"><span data-stu-id="b01c1-108">Members</span></span>
|<span data-ttu-id="b01c1-109">Membro</span><span class="sxs-lookup"><span data-stu-id="b01c1-109">Member</span></span>|<span data-ttu-id="b01c1-110">Valor</span><span class="sxs-lookup"><span data-stu-id="b01c1-110">Value</span></span>|<span data-ttu-id="b01c1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b01c1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b01c1-112">unknown</span><span class="sxs-lookup"><span data-stu-id="b01c1-112">unknown</span></span>|<span data-ttu-id="b01c1-113">0</span><span class="sxs-lookup"><span data-stu-id="b01c1-113">0</span></span>|<span data-ttu-id="b01c1-114">O estado de inscrição do dispositivo é desconhecido</span><span class="sxs-lookup"><span data-stu-id="b01c1-114">Device enrollment state is unknown</span></span>|
|<span data-ttu-id="b01c1-115">inscritos</span><span class="sxs-lookup"><span data-stu-id="b01c1-115">enrolled</span></span>|<span data-ttu-id="b01c1-116">1</span><span class="sxs-lookup"><span data-stu-id="b01c1-116">1</span></span>|<span data-ttu-id="b01c1-117">Inscrever-se o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b01c1-117">Device is Enrolled.</span></span>|
|<span data-ttu-id="b01c1-118">pendingReset</span><span class="sxs-lookup"><span data-stu-id="b01c1-118">pendingReset</span></span>|<span data-ttu-id="b01c1-119">2</span><span class="sxs-lookup"><span data-stu-id="b01c1-119">2</span></span>|<span data-ttu-id="b01c1-120">Inscritos, mas ele está inscrito via perfil de inscrição e o perfil registrado é diferente do perfil atribuído.</span><span class="sxs-lookup"><span data-stu-id="b01c1-120">Enrolled but it's enrolled via enrollment profile and the enrolled profile is different from the assigned profile.</span></span>|
|<span data-ttu-id="b01c1-121">Falha</span><span class="sxs-lookup"><span data-stu-id="b01c1-121">failed</span></span>|<span data-ttu-id="b01c1-122">3</span><span class="sxs-lookup"><span data-stu-id="b01c1-122">3</span></span>|<span data-ttu-id="b01c1-123">Não inscritos e não houver registro de falha de inscrição.</span><span class="sxs-lookup"><span data-stu-id="b01c1-123">Not enrolled and there is enrollment failure record.</span></span>|
|<span data-ttu-id="b01c1-124">notContacted</span><span class="sxs-lookup"><span data-stu-id="b01c1-124">notContacted</span></span>|<span data-ttu-id="b01c1-125">4</span><span class="sxs-lookup"><span data-stu-id="b01c1-125">4</span></span>|<span data-ttu-id="b01c1-126">Dispositivo é importado, mas não inscritos.</span><span class="sxs-lookup"><span data-stu-id="b01c1-126">Device is imported but not enrolled.</span></span>|
|<span data-ttu-id="b01c1-127">bloqueado</span><span class="sxs-lookup"><span data-stu-id="b01c1-127">blocked</span></span>|<span data-ttu-id="b01c1-128">5</span><span class="sxs-lookup"><span data-stu-id="b01c1-128">5</span></span>|<span data-ttu-id="b01c1-129">Dispositivo está inscrito como userless, mas seja bloqueado para mover para a inscrição do usuário porque o aplicativo falha na instalação.</span><span class="sxs-lookup"><span data-stu-id="b01c1-129">Device is enrolled as userless, but is blocked from moving to user enrollment because the app failed to install.</span></span>|





