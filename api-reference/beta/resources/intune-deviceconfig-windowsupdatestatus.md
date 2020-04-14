---
title: tipo de enumeração windowsUpdateStatus
description: Estados do dispositivo de configuração do Windows Update para empresas
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ac307aae8f43cd423c41c1a20ccbc7b9928452d3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43441090"
---
# <a name="windowsupdatestatus-enum-type"></a><span data-ttu-id="10ec4-103">tipo de enumeração windowsUpdateStatus</span><span class="sxs-lookup"><span data-stu-id="10ec4-103">windowsUpdateStatus enum type</span></span>

<span data-ttu-id="10ec4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10ec4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="10ec4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="10ec4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="10ec4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="10ec4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10ec4-107">Estados do dispositivo de configuração do Windows Update para empresas</span><span class="sxs-lookup"><span data-stu-id="10ec4-107">Windows update for business configuration device states</span></span>

## <a name="members"></a><span data-ttu-id="10ec4-108">Membros</span><span class="sxs-lookup"><span data-stu-id="10ec4-108">Members</span></span>
|<span data-ttu-id="10ec4-109">Membro</span><span class="sxs-lookup"><span data-stu-id="10ec4-109">Member</span></span>|<span data-ttu-id="10ec4-110">Valor</span><span class="sxs-lookup"><span data-stu-id="10ec4-110">Value</span></span>|<span data-ttu-id="10ec4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="10ec4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10ec4-112">upToDate</span><span class="sxs-lookup"><span data-stu-id="10ec4-112">upToDate</span></span>|<span data-ttu-id="10ec4-113">,0</span><span class="sxs-lookup"><span data-stu-id="10ec4-113">0</span></span>|<span data-ttu-id="10ec4-114">Não há atualizações pendentes, nenhuma atualização de reinicialização pendente e nenhuma atualização com falha.</span><span class="sxs-lookup"><span data-stu-id="10ec4-114">There are no pending updates, no pending reboot updates and no failed updates.</span></span>|
|<span data-ttu-id="10ec4-115">pendingInstallation</span><span class="sxs-lookup"><span data-stu-id="10ec4-115">pendingInstallation</span></span>|<span data-ttu-id="10ec4-116">1</span><span class="sxs-lookup"><span data-stu-id="10ec4-116">1</span></span>|<span data-ttu-id="10ec4-117">Há atualizações com instalação pendente que inclui atualizações que não foram aprovadas.</span><span class="sxs-lookup"><span data-stu-id="10ec4-117">There are updates that’s pending installation which includes updates that are not approved.</span></span> <span data-ttu-id="10ec4-118">Não há atualizações de reinicialização pendentes, não há atualizações com falha.</span><span class="sxs-lookup"><span data-stu-id="10ec4-118">There are no Pending reboot updates, no failed updates.</span></span>|
|<span data-ttu-id="10ec4-119">pendingReboot</span><span class="sxs-lookup"><span data-stu-id="10ec4-119">pendingReboot</span></span>|<span data-ttu-id="10ec4-120">duas</span><span class="sxs-lookup"><span data-stu-id="10ec4-120">2</span></span>|<span data-ttu-id="10ec4-121">Há atualizações que exigem reinicialização.</span><span class="sxs-lookup"><span data-stu-id="10ec4-121">There are updates that requires reboot.</span></span> <span data-ttu-id="10ec4-122">Não há atualizações com falha.</span><span class="sxs-lookup"><span data-stu-id="10ec4-122">There are not failed updates.</span></span>|
|<span data-ttu-id="10ec4-123">falhou</span><span class="sxs-lookup"><span data-stu-id="10ec4-123">failed</span></span>|<span data-ttu-id="10ec4-124">3D</span><span class="sxs-lookup"><span data-stu-id="10ec4-124">3</span></span>|<span data-ttu-id="10ec4-125">Há atualizações que não puderam ser instaladas no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="10ec4-125">There are updates failed to install on the device.</span></span>|



