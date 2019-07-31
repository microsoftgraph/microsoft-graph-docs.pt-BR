---
title: tipo de enumeração windowsUpdateStatus
description: Estados do dispositivo de configuração do Windows Update para empresas
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 331651bd52988bd8f5503f86e0366c0e5a5a9f22
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968698"
---
# <a name="windowsupdatestatus-enum-type"></a><span data-ttu-id="f85d1-103">tipo de enumeração windowsUpdateStatus</span><span class="sxs-lookup"><span data-stu-id="f85d1-103">windowsUpdateStatus enum type</span></span>

> <span data-ttu-id="f85d1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f85d1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f85d1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f85d1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f85d1-106">Estados do dispositivo de configuração do Windows Update para empresas</span><span class="sxs-lookup"><span data-stu-id="f85d1-106">Windows update for business configuration device states</span></span>

## <a name="members"></a><span data-ttu-id="f85d1-107">Membros</span><span class="sxs-lookup"><span data-stu-id="f85d1-107">Members</span></span>
|<span data-ttu-id="f85d1-108">Membro</span><span class="sxs-lookup"><span data-stu-id="f85d1-108">Member</span></span>|<span data-ttu-id="f85d1-109">Valor</span><span class="sxs-lookup"><span data-stu-id="f85d1-109">Value</span></span>|<span data-ttu-id="f85d1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f85d1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f85d1-111">upToDate</span><span class="sxs-lookup"><span data-stu-id="f85d1-111">upToDate</span></span>|<span data-ttu-id="f85d1-112">,0</span><span class="sxs-lookup"><span data-stu-id="f85d1-112">0</span></span>|<span data-ttu-id="f85d1-113">Não há atualizações pendentes, nenhuma atualização de reinicialização pendente e nenhuma atualização com falha.</span><span class="sxs-lookup"><span data-stu-id="f85d1-113">There are no pending updates, no pending reboot updates and no failed updates.</span></span>|
|<span data-ttu-id="f85d1-114">pendingInstallation</span><span class="sxs-lookup"><span data-stu-id="f85d1-114">pendingInstallation</span></span>|<span data-ttu-id="f85d1-115">1</span><span class="sxs-lookup"><span data-stu-id="f85d1-115">1</span></span>|<span data-ttu-id="f85d1-116">Há atualizações com instalação pendente que inclui atualizações que não foram aprovadas.</span><span class="sxs-lookup"><span data-stu-id="f85d1-116">There are updates that’s pending installation which includes updates that are not approved.</span></span> <span data-ttu-id="f85d1-117">Não há atualizações de reinicialização pendentes, não há atualizações com falha.</span><span class="sxs-lookup"><span data-stu-id="f85d1-117">There are no Pending reboot updates, no failed updates.</span></span>|
|<span data-ttu-id="f85d1-118">pendingReboot</span><span class="sxs-lookup"><span data-stu-id="f85d1-118">pendingReboot</span></span>|<span data-ttu-id="f85d1-119">duas</span><span class="sxs-lookup"><span data-stu-id="f85d1-119">2</span></span>|<span data-ttu-id="f85d1-120">Há atualizações que exigem reinicialização.</span><span class="sxs-lookup"><span data-stu-id="f85d1-120">There are updates that requires reboot.</span></span> <span data-ttu-id="f85d1-121">Não há atualizações com falha.</span><span class="sxs-lookup"><span data-stu-id="f85d1-121">There are not failed updates.</span></span>|
|<span data-ttu-id="f85d1-122">falhou</span><span class="sxs-lookup"><span data-stu-id="f85d1-122">failed</span></span>|<span data-ttu-id="f85d1-123">3D</span><span class="sxs-lookup"><span data-stu-id="f85d1-123">3</span></span>|<span data-ttu-id="f85d1-124">Há atualizações que não puderam ser instaladas no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f85d1-124">There are updates failed to install on the device.</span></span>|





