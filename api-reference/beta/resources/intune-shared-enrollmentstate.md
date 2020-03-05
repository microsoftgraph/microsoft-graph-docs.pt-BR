---
title: tipo de enumeração de enrollmentid
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3002fd793020213f8787f0c62b1e7d7c1c9ee0e5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523678"
---
# <a name="enrollmentstate-enum-type"></a><span data-ttu-id="687c4-103">tipo de enumeração de enrollmentid</span><span class="sxs-lookup"><span data-stu-id="687c4-103">enrollmentState enum type</span></span>

<span data-ttu-id="687c4-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="687c4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="687c4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="687c4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="687c4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="687c4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="687c4-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="687c4-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="687c4-108">Membros</span><span class="sxs-lookup"><span data-stu-id="687c4-108">Members</span></span>
|<span data-ttu-id="687c4-109">Membro</span><span class="sxs-lookup"><span data-stu-id="687c4-109">Member</span></span>|<span data-ttu-id="687c4-110">Valor</span><span class="sxs-lookup"><span data-stu-id="687c4-110">Value</span></span>|<span data-ttu-id="687c4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="687c4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="687c4-112">desconhecido</span><span class="sxs-lookup"><span data-stu-id="687c4-112">unknown</span></span>|<span data-ttu-id="687c4-113">,0</span><span class="sxs-lookup"><span data-stu-id="687c4-113">0</span></span>|<span data-ttu-id="687c4-114">O estado do registro do dispositivo é desconhecido</span><span class="sxs-lookup"><span data-stu-id="687c4-114">Device enrollment state is unknown</span></span>|
|<span data-ttu-id="687c4-115">registrados</span><span class="sxs-lookup"><span data-stu-id="687c4-115">enrolled</span></span>|<span data-ttu-id="687c4-116">1 </span><span class="sxs-lookup"><span data-stu-id="687c4-116">1</span></span>|<span data-ttu-id="687c4-117">O dispositivo está inscrito.</span><span class="sxs-lookup"><span data-stu-id="687c4-117">Device is Enrolled.</span></span>|
|<span data-ttu-id="687c4-118">pendingReset</span><span class="sxs-lookup"><span data-stu-id="687c4-118">pendingReset</span></span>|<span data-ttu-id="687c4-119">2 </span><span class="sxs-lookup"><span data-stu-id="687c4-119">2</span></span>|<span data-ttu-id="687c4-120">Inscrito, mas ele está inscrito via perfil de registro e o perfil inscrito é diferente do perfil atribuído.</span><span class="sxs-lookup"><span data-stu-id="687c4-120">Enrolled but it's enrolled via enrollment profile and the enrolled profile is different from the assigned profile.</span></span>|
|<span data-ttu-id="687c4-121">falhou</span><span class="sxs-lookup"><span data-stu-id="687c4-121">failed</span></span>|<span data-ttu-id="687c4-122">3 </span><span class="sxs-lookup"><span data-stu-id="687c4-122">3</span></span>|<span data-ttu-id="687c4-123">Não registrado e o registro de falha de registro.</span><span class="sxs-lookup"><span data-stu-id="687c4-123">Not enrolled and there is enrollment failure record.</span></span>|
|<span data-ttu-id="687c4-124">Não contatado</span><span class="sxs-lookup"><span data-stu-id="687c4-124">notContacted</span></span>|<span data-ttu-id="687c4-125">4 </span><span class="sxs-lookup"><span data-stu-id="687c4-125">4</span></span>|<span data-ttu-id="687c4-126">O dispositivo é importado, mas não está inscrito.</span><span class="sxs-lookup"><span data-stu-id="687c4-126">Device is imported but not enrolled.</span></span>|
|<span data-ttu-id="687c4-127">bloqueou</span><span class="sxs-lookup"><span data-stu-id="687c4-127">blocked</span></span>|<span data-ttu-id="687c4-128">5 </span><span class="sxs-lookup"><span data-stu-id="687c4-128">5</span></span>|<span data-ttu-id="687c4-129">O dispositivo está inscrito como um não-usuário, mas é impedido de migrar para o registro do usuário porque o aplicativo não pôde ser instalado.</span><span class="sxs-lookup"><span data-stu-id="687c4-129">Device is enrolled as userless, but is blocked from moving to user enrollment because the app failed to install.</span></span>|



