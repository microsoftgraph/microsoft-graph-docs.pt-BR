---
title: tipo de enumeração de enrollmentid
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: da96d5e0f1b86057178755bbd4e0761f49220095
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48084293"
---
# <a name="enrollmentstate-enum-type"></a><span data-ttu-id="aef86-103">tipo de enumeração de enrollmentid</span><span class="sxs-lookup"><span data-stu-id="aef86-103">enrollmentState enum type</span></span>

<span data-ttu-id="aef86-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aef86-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aef86-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="aef86-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aef86-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aef86-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aef86-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="aef86-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="aef86-108">Membros</span><span class="sxs-lookup"><span data-stu-id="aef86-108">Members</span></span>
|<span data-ttu-id="aef86-109">Membro</span><span class="sxs-lookup"><span data-stu-id="aef86-109">Member</span></span>|<span data-ttu-id="aef86-110">Valor</span><span class="sxs-lookup"><span data-stu-id="aef86-110">Value</span></span>|<span data-ttu-id="aef86-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="aef86-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aef86-112">desconhecido</span><span class="sxs-lookup"><span data-stu-id="aef86-112">unknown</span></span>|<span data-ttu-id="aef86-113">,0</span><span class="sxs-lookup"><span data-stu-id="aef86-113">0</span></span>|<span data-ttu-id="aef86-114">O estado do registro do dispositivo é desconhecido</span><span class="sxs-lookup"><span data-stu-id="aef86-114">Device enrollment state is unknown</span></span>|
|<span data-ttu-id="aef86-115">registrados</span><span class="sxs-lookup"><span data-stu-id="aef86-115">enrolled</span></span>|<span data-ttu-id="aef86-116">1 </span><span class="sxs-lookup"><span data-stu-id="aef86-116">1</span></span>|<span data-ttu-id="aef86-117">O dispositivo está inscrito.</span><span class="sxs-lookup"><span data-stu-id="aef86-117">Device is Enrolled.</span></span>|
|<span data-ttu-id="aef86-118">pendingReset</span><span class="sxs-lookup"><span data-stu-id="aef86-118">pendingReset</span></span>|<span data-ttu-id="aef86-119">2 </span><span class="sxs-lookup"><span data-stu-id="aef86-119">2</span></span>|<span data-ttu-id="aef86-120">Inscrito, mas ele está inscrito via perfil de registro e o perfil inscrito é diferente do perfil atribuído.</span><span class="sxs-lookup"><span data-stu-id="aef86-120">Enrolled but it's enrolled via enrollment profile and the enrolled profile is different from the assigned profile.</span></span>|
|<span data-ttu-id="aef86-121">falhou</span><span class="sxs-lookup"><span data-stu-id="aef86-121">failed</span></span>|<span data-ttu-id="aef86-122">3D</span><span class="sxs-lookup"><span data-stu-id="aef86-122">3</span></span>|<span data-ttu-id="aef86-123">Não registrado e o registro de falha de registro.</span><span class="sxs-lookup"><span data-stu-id="aef86-123">Not enrolled and there is enrollment failure record.</span></span>|
|<span data-ttu-id="aef86-124">Não contatado</span><span class="sxs-lookup"><span data-stu-id="aef86-124">notContacted</span></span>|<span data-ttu-id="aef86-125">4 </span><span class="sxs-lookup"><span data-stu-id="aef86-125">4</span></span>|<span data-ttu-id="aef86-126">O dispositivo é importado, mas não está inscrito.</span><span class="sxs-lookup"><span data-stu-id="aef86-126">Device is imported but not enrolled.</span></span>|
|<span data-ttu-id="aef86-127">bloqueou</span><span class="sxs-lookup"><span data-stu-id="aef86-127">blocked</span></span>|<span data-ttu-id="aef86-128">5 </span><span class="sxs-lookup"><span data-stu-id="aef86-128">5</span></span>|<span data-ttu-id="aef86-129">O dispositivo está inscrito como um não-usuário, mas é impedido de migrar para o registro do usuário porque o aplicativo não pôde ser instalado.</span><span class="sxs-lookup"><span data-stu-id="aef86-129">Device is enrolled as userless, but is blocked from moving to user enrollment because the app failed to install.</span></span>|






