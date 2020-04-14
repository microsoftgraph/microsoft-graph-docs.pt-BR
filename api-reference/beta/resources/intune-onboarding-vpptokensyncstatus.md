---
title: tipo de enumeração vppTokenSyncStatus
description: Possíveis status de sincronização associados a um token do Apple Volume Purchase Program.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 28ec478d33ddeb5c56963bf6c750a98ab217cc75
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43446805"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="0f25e-103">tipo de enumeração vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="0f25e-103">vppTokenSyncStatus enum type</span></span>

<span data-ttu-id="0f25e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f25e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0f25e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0f25e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f25e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0f25e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f25e-107">Possíveis status de sincronização associados a um token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="0f25e-107">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="0f25e-108">Membros</span><span class="sxs-lookup"><span data-stu-id="0f25e-108">Members</span></span>
|<span data-ttu-id="0f25e-109">Membro</span><span class="sxs-lookup"><span data-stu-id="0f25e-109">Member</span></span>|<span data-ttu-id="0f25e-110">Valor</span><span class="sxs-lookup"><span data-stu-id="0f25e-110">Value</span></span>|<span data-ttu-id="0f25e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0f25e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f25e-112">nenhuma</span><span class="sxs-lookup"><span data-stu-id="0f25e-112">none</span></span>|<span data-ttu-id="0f25e-113">,0</span><span class="sxs-lookup"><span data-stu-id="0f25e-113">0</span></span>|<span data-ttu-id="0f25e-114">Status padrão.</span><span class="sxs-lookup"><span data-stu-id="0f25e-114">Default status.</span></span>|
|<span data-ttu-id="0f25e-115">inProgress</span><span class="sxs-lookup"><span data-stu-id="0f25e-115">inProgress</span></span>|<span data-ttu-id="0f25e-116">1</span><span class="sxs-lookup"><span data-stu-id="0f25e-116">1</span></span>|<span data-ttu-id="0f25e-117">Última sincronização em andamento.</span><span class="sxs-lookup"><span data-stu-id="0f25e-117">Last Sync in progress.</span></span>|
|<span data-ttu-id="0f25e-118">Completed</span><span class="sxs-lookup"><span data-stu-id="0f25e-118">completed</span></span>|<span data-ttu-id="0f25e-119">duas</span><span class="sxs-lookup"><span data-stu-id="0f25e-119">2</span></span>|<span data-ttu-id="0f25e-120">Última sincronização concluída com êxito.</span><span class="sxs-lookup"><span data-stu-id="0f25e-120">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="0f25e-121">falhou</span><span class="sxs-lookup"><span data-stu-id="0f25e-121">failed</span></span>|<span data-ttu-id="0f25e-122">3D</span><span class="sxs-lookup"><span data-stu-id="0f25e-122">3</span></span>|<span data-ttu-id="0f25e-123">Falha na última sincronização.</span><span class="sxs-lookup"><span data-stu-id="0f25e-123">Last Sync failed.</span></span>|



