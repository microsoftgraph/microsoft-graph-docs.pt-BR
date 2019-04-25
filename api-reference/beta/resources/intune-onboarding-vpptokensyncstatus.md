---
title: tipo de enumeração vppTokenSyncStatus
description: Possíveis status de sincronização associados a um token do Apple Volume Purchase Program.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 59653a8df6c0fd08ffd0d8aa3081d58e56447a95
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566371"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="71194-103">tipo de enumeração vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="71194-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="71194-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="71194-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71194-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="71194-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71194-106">Possíveis status de sincronização associados a um token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="71194-106">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="71194-107">Membros</span><span class="sxs-lookup"><span data-stu-id="71194-107">Members</span></span>
|<span data-ttu-id="71194-108">Membro</span><span class="sxs-lookup"><span data-stu-id="71194-108">Member</span></span>|<span data-ttu-id="71194-109">Valor</span><span class="sxs-lookup"><span data-stu-id="71194-109">Value</span></span>|<span data-ttu-id="71194-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="71194-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71194-111">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="71194-111">none</span></span>|<span data-ttu-id="71194-112">,0</span><span class="sxs-lookup"><span data-stu-id="71194-112">0</span></span>|<span data-ttu-id="71194-113">Status padrão.</span><span class="sxs-lookup"><span data-stu-id="71194-113">Default status.</span></span>|
|<span data-ttu-id="71194-114">inProgress</span><span class="sxs-lookup"><span data-stu-id="71194-114">inProgress</span></span>|<span data-ttu-id="71194-115">1 </span><span class="sxs-lookup"><span data-stu-id="71194-115">1</span></span>|<span data-ttu-id="71194-116">Última sincronização em andamento.</span><span class="sxs-lookup"><span data-stu-id="71194-116">Last Sync in progress.</span></span>|
|<span data-ttu-id="71194-117">Completed</span><span class="sxs-lookup"><span data-stu-id="71194-117">completed</span></span>|<span data-ttu-id="71194-118">2 </span><span class="sxs-lookup"><span data-stu-id="71194-118">2</span></span>|<span data-ttu-id="71194-119">Última sincronização concluída com êxito.</span><span class="sxs-lookup"><span data-stu-id="71194-119">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="71194-120">falhou</span><span class="sxs-lookup"><span data-stu-id="71194-120">failed</span></span>|<span data-ttu-id="71194-121">3 </span><span class="sxs-lookup"><span data-stu-id="71194-121">3</span></span>|<span data-ttu-id="71194-122">Falha na última sincronização.</span><span class="sxs-lookup"><span data-stu-id="71194-122">Last Sync failed.</span></span>|





