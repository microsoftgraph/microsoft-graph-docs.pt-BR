---
title: tipo de enumeração windowsUpdateStatus
description: Estados do dispositivo de configuração do Windows Update para empresas
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3a09aca9ce1ac4cd81e09b8db8da10ea563f1f03
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49272364"
---
# <a name="windowsupdatestatus-enum-type"></a><span data-ttu-id="d073d-103">tipo de enumeração windowsUpdateStatus</span><span class="sxs-lookup"><span data-stu-id="d073d-103">windowsUpdateStatus enum type</span></span>

<span data-ttu-id="d073d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d073d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d073d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d073d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d073d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d073d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d073d-107">Estados do dispositivo de configuração do Windows Update para empresas</span><span class="sxs-lookup"><span data-stu-id="d073d-107">Windows update for business configuration device states</span></span>

## <a name="members"></a><span data-ttu-id="d073d-108">Membros</span><span class="sxs-lookup"><span data-stu-id="d073d-108">Members</span></span>
|<span data-ttu-id="d073d-109">Membro</span><span class="sxs-lookup"><span data-stu-id="d073d-109">Member</span></span>|<span data-ttu-id="d073d-110">Valor</span><span class="sxs-lookup"><span data-stu-id="d073d-110">Value</span></span>|<span data-ttu-id="d073d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d073d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d073d-112">upToDate</span><span class="sxs-lookup"><span data-stu-id="d073d-112">upToDate</span></span>|<span data-ttu-id="d073d-113">,0</span><span class="sxs-lookup"><span data-stu-id="d073d-113">0</span></span>|<span data-ttu-id="d073d-114">Não há atualizações pendentes, nenhuma atualização de reinicialização pendente e nenhuma atualização com falha.</span><span class="sxs-lookup"><span data-stu-id="d073d-114">There are no pending updates, no pending reboot updates and no failed updates.</span></span>|
|<span data-ttu-id="d073d-115">pendingInstallation</span><span class="sxs-lookup"><span data-stu-id="d073d-115">pendingInstallation</span></span>|<span data-ttu-id="d073d-116">1</span><span class="sxs-lookup"><span data-stu-id="d073d-116">1</span></span>|<span data-ttu-id="d073d-117">Há atualizações com instalação pendente que inclui atualizações que não foram aprovadas.</span><span class="sxs-lookup"><span data-stu-id="d073d-117">There are updates that’s pending installation which includes updates that are not approved.</span></span> <span data-ttu-id="d073d-118">Não há atualizações de reinicialização pendentes, não há atualizações com falha.</span><span class="sxs-lookup"><span data-stu-id="d073d-118">There are no Pending reboot updates, no failed updates.</span></span>|
|<span data-ttu-id="d073d-119">pendingReboot</span><span class="sxs-lookup"><span data-stu-id="d073d-119">pendingReboot</span></span>|<span data-ttu-id="d073d-120">duas</span><span class="sxs-lookup"><span data-stu-id="d073d-120">2</span></span>|<span data-ttu-id="d073d-121">Há atualizações que exigem reinicialização.</span><span class="sxs-lookup"><span data-stu-id="d073d-121">There are updates that requires reboot.</span></span> <span data-ttu-id="d073d-122">Não há atualizações com falha.</span><span class="sxs-lookup"><span data-stu-id="d073d-122">There are not failed updates.</span></span>|
|<span data-ttu-id="d073d-123">falhou</span><span class="sxs-lookup"><span data-stu-id="d073d-123">failed</span></span>|<span data-ttu-id="d073d-124">3D</span><span class="sxs-lookup"><span data-stu-id="d073d-124">3</span></span>|<span data-ttu-id="d073d-125">Há atualizações que não puderam ser instaladas no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d073d-125">There are updates failed to install on the device.</span></span>|




