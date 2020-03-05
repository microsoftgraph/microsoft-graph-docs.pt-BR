---
title: tipo de enumeração vppTokenSyncStatus
description: Possíveis status de sincronização associados a um token do Apple Volume Purchase Program.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: a9955b825fffab7837cb2c77ffa443ad3f9c9fa1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524059"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="1b49d-103">tipo de enumeração vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="1b49d-103">vppTokenSyncStatus enum type</span></span>

<span data-ttu-id="1b49d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1b49d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1b49d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1b49d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b49d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1b49d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b49d-107">Possíveis status de sincronização associados a um token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="1b49d-107">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="1b49d-108">Membros</span><span class="sxs-lookup"><span data-stu-id="1b49d-108">Members</span></span>
|<span data-ttu-id="1b49d-109">Membro</span><span class="sxs-lookup"><span data-stu-id="1b49d-109">Member</span></span>|<span data-ttu-id="1b49d-110">Valor</span><span class="sxs-lookup"><span data-stu-id="1b49d-110">Value</span></span>|<span data-ttu-id="1b49d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b49d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b49d-112">nenhuma</span><span class="sxs-lookup"><span data-stu-id="1b49d-112">none</span></span>|<span data-ttu-id="1b49d-113">,0</span><span class="sxs-lookup"><span data-stu-id="1b49d-113">0</span></span>|<span data-ttu-id="1b49d-114">Status padrão.</span><span class="sxs-lookup"><span data-stu-id="1b49d-114">Default status.</span></span>|
|<span data-ttu-id="1b49d-115">inProgress</span><span class="sxs-lookup"><span data-stu-id="1b49d-115">inProgress</span></span>|<span data-ttu-id="1b49d-116">1 </span><span class="sxs-lookup"><span data-stu-id="1b49d-116">1</span></span>|<span data-ttu-id="1b49d-117">Última sincronização em andamento.</span><span class="sxs-lookup"><span data-stu-id="1b49d-117">Last Sync in progress.</span></span>|
|<span data-ttu-id="1b49d-118">Completed</span><span class="sxs-lookup"><span data-stu-id="1b49d-118">completed</span></span>|<span data-ttu-id="1b49d-119">2 </span><span class="sxs-lookup"><span data-stu-id="1b49d-119">2</span></span>|<span data-ttu-id="1b49d-120">Última sincronização concluída com êxito.</span><span class="sxs-lookup"><span data-stu-id="1b49d-120">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="1b49d-121">falhou</span><span class="sxs-lookup"><span data-stu-id="1b49d-121">failed</span></span>|<span data-ttu-id="1b49d-122">3 </span><span class="sxs-lookup"><span data-stu-id="1b49d-122">3</span></span>|<span data-ttu-id="1b49d-123">Falha na última sincronização.</span><span class="sxs-lookup"><span data-stu-id="1b49d-123">Last Sync failed.</span></span>|



