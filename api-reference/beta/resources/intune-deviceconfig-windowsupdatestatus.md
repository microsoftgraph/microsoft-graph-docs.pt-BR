---
title: tipo de enumeração windowsUpdateStatus
description: Estados do dispositivo de configuração do Windows Update para empresas
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 73cd3208b7729544d6fbd620a13ce295b39aff26
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523620"
---
# <a name="windowsupdatestatus-enum-type"></a><span data-ttu-id="06999-103">tipo de enumeração windowsUpdateStatus</span><span class="sxs-lookup"><span data-stu-id="06999-103">windowsUpdateStatus enum type</span></span>

> <span data-ttu-id="06999-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="06999-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06999-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="06999-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06999-106">Estados do dispositivo de configuração do Windows Update para empresas</span><span class="sxs-lookup"><span data-stu-id="06999-106">Windows update for business configuration device states</span></span>

## <a name="members"></a><span data-ttu-id="06999-107">Membros</span><span class="sxs-lookup"><span data-stu-id="06999-107">Members</span></span>
|<span data-ttu-id="06999-108">Membro</span><span class="sxs-lookup"><span data-stu-id="06999-108">Member</span></span>|<span data-ttu-id="06999-109">Valor</span><span class="sxs-lookup"><span data-stu-id="06999-109">Value</span></span>|<span data-ttu-id="06999-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="06999-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06999-111">upToDate</span><span class="sxs-lookup"><span data-stu-id="06999-111">upToDate</span></span>|<span data-ttu-id="06999-112">,0</span><span class="sxs-lookup"><span data-stu-id="06999-112">0</span></span>|<span data-ttu-id="06999-113">Não há atualizações pendentes, nenhuma atualização de reinicialização pendente e nenhuma atualização com falha.</span><span class="sxs-lookup"><span data-stu-id="06999-113">There are no pending updates, no pending reboot updates and no failed updates.</span></span>|
|<span data-ttu-id="06999-114">pendingInstallation</span><span class="sxs-lookup"><span data-stu-id="06999-114">pendingInstallation</span></span>|<span data-ttu-id="06999-115">1 </span><span class="sxs-lookup"><span data-stu-id="06999-115">1</span></span>|<span data-ttu-id="06999-116">Há atualizações com instalação pendente que inclui atualizações que não foram aprovadas.</span><span class="sxs-lookup"><span data-stu-id="06999-116">There are updates that’s pending installation which includes updates that are not approved.</span></span> <span data-ttu-id="06999-117">Não há atualizações de reinicialização pendentes, não há atualizações com falha.</span><span class="sxs-lookup"><span data-stu-id="06999-117">There are no Pending reboot updates, no failed updates.</span></span>|
|<span data-ttu-id="06999-118">pendingReboot</span><span class="sxs-lookup"><span data-stu-id="06999-118">pendingReboot</span></span>|<span data-ttu-id="06999-119">2 </span><span class="sxs-lookup"><span data-stu-id="06999-119">2</span></span>|<span data-ttu-id="06999-120">Há atualizações que exigem reinicialização.</span><span class="sxs-lookup"><span data-stu-id="06999-120">There are updates that requires reboot.</span></span> <span data-ttu-id="06999-121">Não há atualizações com falha.</span><span class="sxs-lookup"><span data-stu-id="06999-121">There are not failed updates.</span></span>|
|<span data-ttu-id="06999-122">falhou</span><span class="sxs-lookup"><span data-stu-id="06999-122">failed</span></span>|<span data-ttu-id="06999-123">3 </span><span class="sxs-lookup"><span data-stu-id="06999-123">3</span></span>|<span data-ttu-id="06999-124">Há atualizações que não puderam ser instaladas no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="06999-124">There are updates failed to install on the device.</span></span>|





