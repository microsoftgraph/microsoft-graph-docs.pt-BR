---
title: tipo de enumeração windowsUpdateStatus
description: Estados do dispositivo de configuração do Windows Update para empresas
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c6eecee6626e4d47856071de3ebb53944e196478
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943638"
---
# <a name="windowsupdatestatus-enum-type"></a><span data-ttu-id="d74bd-103">tipo de enumeração windowsUpdateStatus</span><span class="sxs-lookup"><span data-stu-id="d74bd-103">windowsUpdateStatus enum type</span></span>

> <span data-ttu-id="d74bd-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d74bd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d74bd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d74bd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d74bd-106">Estados do dispositivo de configuração do Windows Update para empresas</span><span class="sxs-lookup"><span data-stu-id="d74bd-106">Windows update for business configuration device states</span></span>

## <a name="members"></a><span data-ttu-id="d74bd-107">Membros</span><span class="sxs-lookup"><span data-stu-id="d74bd-107">Members</span></span>
|<span data-ttu-id="d74bd-108">Membro</span><span class="sxs-lookup"><span data-stu-id="d74bd-108">Member</span></span>|<span data-ttu-id="d74bd-109">Valor</span><span class="sxs-lookup"><span data-stu-id="d74bd-109">Value</span></span>|<span data-ttu-id="d74bd-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d74bd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d74bd-111">upToDate</span><span class="sxs-lookup"><span data-stu-id="d74bd-111">upToDate</span></span>|<span data-ttu-id="d74bd-112">,0</span><span class="sxs-lookup"><span data-stu-id="d74bd-112">0</span></span>|<span data-ttu-id="d74bd-113">Não há atualizações pendentes, nenhuma atualização de reinicialização pendente e nenhuma atualização com falha.</span><span class="sxs-lookup"><span data-stu-id="d74bd-113">There are no pending updates, no pending reboot updates and no failed updates.</span></span>|
|<span data-ttu-id="d74bd-114">pendingInstallation</span><span class="sxs-lookup"><span data-stu-id="d74bd-114">pendingInstallation</span></span>|<span data-ttu-id="d74bd-115">1</span><span class="sxs-lookup"><span data-stu-id="d74bd-115">1</span></span>|<span data-ttu-id="d74bd-116">Há atualizações com instalação pendente que inclui atualizações que não foram aprovadas.</span><span class="sxs-lookup"><span data-stu-id="d74bd-116">There are updates that’s pending installation which includes updates that are not approved.</span></span> <span data-ttu-id="d74bd-117">Não há atualizações de reinicialização pendentes, não há atualizações com falha.</span><span class="sxs-lookup"><span data-stu-id="d74bd-117">There are no Pending reboot updates, no failed updates.</span></span>|
|<span data-ttu-id="d74bd-118">pendingReboot</span><span class="sxs-lookup"><span data-stu-id="d74bd-118">pendingReboot</span></span>|<span data-ttu-id="d74bd-119">duas</span><span class="sxs-lookup"><span data-stu-id="d74bd-119">2</span></span>|<span data-ttu-id="d74bd-120">Há atualizações que exigem reinicialização.</span><span class="sxs-lookup"><span data-stu-id="d74bd-120">There are updates that requires reboot.</span></span> <span data-ttu-id="d74bd-121">Não há atualizações com falha.</span><span class="sxs-lookup"><span data-stu-id="d74bd-121">There are not failed updates.</span></span>|
|<span data-ttu-id="d74bd-122">falhou</span><span class="sxs-lookup"><span data-stu-id="d74bd-122">failed</span></span>|<span data-ttu-id="d74bd-123">3D</span><span class="sxs-lookup"><span data-stu-id="d74bd-123">3</span></span>|<span data-ttu-id="d74bd-124">Há atualizações que não puderam ser instaladas no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d74bd-124">There are updates failed to install on the device.</span></span>|




