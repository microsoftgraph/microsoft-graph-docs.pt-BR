---
title: tipo de enumeração windowsUpdateStatus
description: Estados do dispositivo de configuração do Windows Update para empresas
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 90fb42248dc0bc78e33c18150b59d88487a6a06b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525366"
---
# <a name="windowsupdatestatus-enum-type"></a><span data-ttu-id="e62ba-103">tipo de enumeração windowsUpdateStatus</span><span class="sxs-lookup"><span data-stu-id="e62ba-103">windowsUpdateStatus enum type</span></span>

<span data-ttu-id="e62ba-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e62ba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e62ba-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e62ba-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e62ba-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e62ba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e62ba-107">Estados do dispositivo de configuração do Windows Update para empresas</span><span class="sxs-lookup"><span data-stu-id="e62ba-107">Windows update for business configuration device states</span></span>

## <a name="members"></a><span data-ttu-id="e62ba-108">Membros</span><span class="sxs-lookup"><span data-stu-id="e62ba-108">Members</span></span>
|<span data-ttu-id="e62ba-109">Membro</span><span class="sxs-lookup"><span data-stu-id="e62ba-109">Member</span></span>|<span data-ttu-id="e62ba-110">Valor</span><span class="sxs-lookup"><span data-stu-id="e62ba-110">Value</span></span>|<span data-ttu-id="e62ba-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e62ba-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e62ba-112">upToDate</span><span class="sxs-lookup"><span data-stu-id="e62ba-112">upToDate</span></span>|<span data-ttu-id="e62ba-113">,0</span><span class="sxs-lookup"><span data-stu-id="e62ba-113">0</span></span>|<span data-ttu-id="e62ba-114">Não há atualizações pendentes, nenhuma atualização de reinicialização pendente e nenhuma atualização com falha.</span><span class="sxs-lookup"><span data-stu-id="e62ba-114">There are no pending updates, no pending reboot updates and no failed updates.</span></span>|
|<span data-ttu-id="e62ba-115">pendingInstallation</span><span class="sxs-lookup"><span data-stu-id="e62ba-115">pendingInstallation</span></span>|<span data-ttu-id="e62ba-116">1 </span><span class="sxs-lookup"><span data-stu-id="e62ba-116">1</span></span>|<span data-ttu-id="e62ba-117">Há atualizações com instalação pendente que inclui atualizações que não foram aprovadas.</span><span class="sxs-lookup"><span data-stu-id="e62ba-117">There are updates that’s pending installation which includes updates that are not approved.</span></span> <span data-ttu-id="e62ba-118">Não há atualizações de reinicialização pendentes, não há atualizações com falha.</span><span class="sxs-lookup"><span data-stu-id="e62ba-118">There are no Pending reboot updates, no failed updates.</span></span>|
|<span data-ttu-id="e62ba-119">pendingReboot</span><span class="sxs-lookup"><span data-stu-id="e62ba-119">pendingReboot</span></span>|<span data-ttu-id="e62ba-120">2 </span><span class="sxs-lookup"><span data-stu-id="e62ba-120">2</span></span>|<span data-ttu-id="e62ba-121">Há atualizações que exigem reinicialização.</span><span class="sxs-lookup"><span data-stu-id="e62ba-121">There are updates that requires reboot.</span></span> <span data-ttu-id="e62ba-122">Não há atualizações com falha.</span><span class="sxs-lookup"><span data-stu-id="e62ba-122">There are not failed updates.</span></span>|
|<span data-ttu-id="e62ba-123">falhou</span><span class="sxs-lookup"><span data-stu-id="e62ba-123">failed</span></span>|<span data-ttu-id="e62ba-124">3 </span><span class="sxs-lookup"><span data-stu-id="e62ba-124">3</span></span>|<span data-ttu-id="e62ba-125">Há atualizações que não puderam ser instaladas no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e62ba-125">There are updates failed to install on the device.</span></span>|



