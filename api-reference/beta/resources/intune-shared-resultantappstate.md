---
title: tipo de enumeração resultantAppState
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5e39426c26f819a73d933c47a296378021d62b2c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48084097"
---
# <a name="resultantappstate-enum-type"></a><span data-ttu-id="b1b47-103">tipo de enumeração resultantAppState</span><span class="sxs-lookup"><span data-stu-id="b1b47-103">resultantAppState enum type</span></span>

<span data-ttu-id="b1b47-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1b47-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b1b47-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b1b47-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1b47-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b1b47-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1b47-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b1b47-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="b1b47-108">Membros</span><span class="sxs-lookup"><span data-stu-id="b1b47-108">Members</span></span>
|<span data-ttu-id="b1b47-109">Membro</span><span class="sxs-lookup"><span data-stu-id="b1b47-109">Member</span></span>|<span data-ttu-id="b1b47-110">Valor</span><span class="sxs-lookup"><span data-stu-id="b1b47-110">Value</span></span>|<span data-ttu-id="b1b47-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1b47-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1b47-112">instalação</span><span class="sxs-lookup"><span data-stu-id="b1b47-112">installed</span></span>|<span data-ttu-id="b1b47-113">1 </span><span class="sxs-lookup"><span data-stu-id="b1b47-113">1</span></span>|<span data-ttu-id="b1b47-114">O aplicativo é instalado sem erros</span><span class="sxs-lookup"><span data-stu-id="b1b47-114">The application is installed with no errors</span></span>|
|<span data-ttu-id="b1b47-115">falhou</span><span class="sxs-lookup"><span data-stu-id="b1b47-115">failed</span></span>|<span data-ttu-id="b1b47-116">2 </span><span class="sxs-lookup"><span data-stu-id="b1b47-116">2</span></span>|<span data-ttu-id="b1b47-117">Falha ao instalar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b1b47-117">The application failed to install.</span></span>|
|<span data-ttu-id="b1b47-118">não instalado</span><span class="sxs-lookup"><span data-stu-id="b1b47-118">notInstalled</span></span>|<span data-ttu-id="b1b47-119">3D</span><span class="sxs-lookup"><span data-stu-id="b1b47-119">3</span></span>|<span data-ttu-id="b1b47-120">O aplicativo não está instalado.</span><span class="sxs-lookup"><span data-stu-id="b1b47-120">The application is not installed.</span></span>|
|<span data-ttu-id="b1b47-121">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="b1b47-121">uninstallFailed</span></span>|<span data-ttu-id="b1b47-122">4 </span><span class="sxs-lookup"><span data-stu-id="b1b47-122">4</span></span>|<span data-ttu-id="b1b47-123">Falha ao desinstalar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b1b47-123">The application failed to uninstall.</span></span>|
|<span data-ttu-id="b1b47-124">pendingInstall</span><span class="sxs-lookup"><span data-stu-id="b1b47-124">pendingInstall</span></span>|<span data-ttu-id="b1b47-125">5 </span><span class="sxs-lookup"><span data-stu-id="b1b47-125">5</span></span>|<span data-ttu-id="b1b47-126">A instalação do aplicativo está em andamento.</span><span class="sxs-lookup"><span data-stu-id="b1b47-126">The installation of the application is in progress.</span></span>|
|<span data-ttu-id="b1b47-127">desconhecido</span><span class="sxs-lookup"><span data-stu-id="b1b47-127">unknown</span></span>|<span data-ttu-id="b1b47-128">99</span><span class="sxs-lookup"><span data-stu-id="b1b47-128">99</span></span>|<span data-ttu-id="b1b47-129">O status do aplicativo é desconhecido.</span><span class="sxs-lookup"><span data-stu-id="b1b47-129">The status of the application is unknown.</span></span>|
|<span data-ttu-id="b1b47-130">Não aplicável</span><span class="sxs-lookup"><span data-stu-id="b1b47-130">notApplicable</span></span>|<span data-ttu-id="b1b47-131">-1</span><span class="sxs-lookup"><span data-stu-id="b1b47-131">-1</span></span>|<span data-ttu-id="b1b47-132">O aplicativo não é aplicável.</span><span class="sxs-lookup"><span data-stu-id="b1b47-132">The application is not applicable.</span></span>|






