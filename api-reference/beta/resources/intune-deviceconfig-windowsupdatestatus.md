---
title: tipo de enumeração windowsUpdateStatus
description: Estados do dispositivo de configuração do Windows Update para empresas
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0151a572011f9033ae7b622e5d3cf2bfd086ed39
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706930"
---
# <a name="windowsupdatestatus-enum-type"></a><span data-ttu-id="7daa8-103">tipo de enumeração windowsUpdateStatus</span><span class="sxs-lookup"><span data-stu-id="7daa8-103">windowsUpdateStatus enum type</span></span>

<span data-ttu-id="7daa8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7daa8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7daa8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7daa8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7daa8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7daa8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7daa8-107">Estados do dispositivo de configuração do Windows Update para empresas</span><span class="sxs-lookup"><span data-stu-id="7daa8-107">Windows update for business configuration device states</span></span>

## <a name="members"></a><span data-ttu-id="7daa8-108">Membros</span><span class="sxs-lookup"><span data-stu-id="7daa8-108">Members</span></span>
|<span data-ttu-id="7daa8-109">Membro</span><span class="sxs-lookup"><span data-stu-id="7daa8-109">Member</span></span>|<span data-ttu-id="7daa8-110">Valor</span><span class="sxs-lookup"><span data-stu-id="7daa8-110">Value</span></span>|<span data-ttu-id="7daa8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7daa8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7daa8-112">upToDate</span><span class="sxs-lookup"><span data-stu-id="7daa8-112">upToDate</span></span>|<span data-ttu-id="7daa8-113">,0</span><span class="sxs-lookup"><span data-stu-id="7daa8-113">0</span></span>|<span data-ttu-id="7daa8-114">Não há atualizações pendentes, nenhuma atualização de reinicialização pendente e nenhuma atualização com falha.</span><span class="sxs-lookup"><span data-stu-id="7daa8-114">There are no pending updates, no pending reboot updates and no failed updates.</span></span>|
|<span data-ttu-id="7daa8-115">pendingInstallation</span><span class="sxs-lookup"><span data-stu-id="7daa8-115">pendingInstallation</span></span>|<span data-ttu-id="7daa8-116">1</span><span class="sxs-lookup"><span data-stu-id="7daa8-116">1</span></span>|<span data-ttu-id="7daa8-117">Há atualizações com instalação pendente que inclui atualizações que não foram aprovadas.</span><span class="sxs-lookup"><span data-stu-id="7daa8-117">There are updates that’s pending installation which includes updates that are not approved.</span></span> <span data-ttu-id="7daa8-118">Não há atualizações de reinicialização pendentes, não há atualizações com falha.</span><span class="sxs-lookup"><span data-stu-id="7daa8-118">There are no Pending reboot updates, no failed updates.</span></span>|
|<span data-ttu-id="7daa8-119">pendingReboot</span><span class="sxs-lookup"><span data-stu-id="7daa8-119">pendingReboot</span></span>|<span data-ttu-id="7daa8-120">duas</span><span class="sxs-lookup"><span data-stu-id="7daa8-120">2</span></span>|<span data-ttu-id="7daa8-121">Há atualizações que exigem reinicialização.</span><span class="sxs-lookup"><span data-stu-id="7daa8-121">There are updates that requires reboot.</span></span> <span data-ttu-id="7daa8-122">Não há atualizações com falha.</span><span class="sxs-lookup"><span data-stu-id="7daa8-122">There are not failed updates.</span></span>|
|<span data-ttu-id="7daa8-123">falhou</span><span class="sxs-lookup"><span data-stu-id="7daa8-123">failed</span></span>|<span data-ttu-id="7daa8-124">3D</span><span class="sxs-lookup"><span data-stu-id="7daa8-124">3</span></span>|<span data-ttu-id="7daa8-125">Há atualizações que não puderam ser instaladas no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="7daa8-125">There are updates failed to install on the device.</span></span>|





