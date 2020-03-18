---
title: tipo de enumeração vppTokenSyncStatus
description: Possíveis status de sincronização associados a um token do Apple Volume Purchase Program.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b298fd52c390d9e926ca9be69e276aac3b6a6de0
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42777254"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="5623e-103">tipo de enumeração vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="5623e-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="5623e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5623e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5623e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5623e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5623e-106">Possíveis status de sincronização associados a um token do Apple Volume Purchase Program.</span><span class="sxs-lookup"><span data-stu-id="5623e-106">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="5623e-107">Membros</span><span class="sxs-lookup"><span data-stu-id="5623e-107">Members</span></span>
|<span data-ttu-id="5623e-108">Membro</span><span class="sxs-lookup"><span data-stu-id="5623e-108">Member</span></span>|<span data-ttu-id="5623e-109">Valor</span><span class="sxs-lookup"><span data-stu-id="5623e-109">Value</span></span>|<span data-ttu-id="5623e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5623e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5623e-111">none</span><span class="sxs-lookup"><span data-stu-id="5623e-111">none</span></span>|<span data-ttu-id="5623e-112">,0</span><span class="sxs-lookup"><span data-stu-id="5623e-112">0</span></span>|<span data-ttu-id="5623e-113">Status padrão.</span><span class="sxs-lookup"><span data-stu-id="5623e-113">Default status.</span></span>|
|<span data-ttu-id="5623e-114">inProgress</span><span class="sxs-lookup"><span data-stu-id="5623e-114">inProgress</span></span>|<span data-ttu-id="5623e-115">1</span><span class="sxs-lookup"><span data-stu-id="5623e-115">1</span></span>|<span data-ttu-id="5623e-116">Última sincronização em andamento.</span><span class="sxs-lookup"><span data-stu-id="5623e-116">Last Sync in progress.</span></span>|
|<span data-ttu-id="5623e-117">Completed</span><span class="sxs-lookup"><span data-stu-id="5623e-117">completed</span></span>|<span data-ttu-id="5623e-118">duas</span><span class="sxs-lookup"><span data-stu-id="5623e-118">2</span></span>|<span data-ttu-id="5623e-119">Última sincronização concluída com êxito.</span><span class="sxs-lookup"><span data-stu-id="5623e-119">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="5623e-120">falhou</span><span class="sxs-lookup"><span data-stu-id="5623e-120">failed</span></span>|<span data-ttu-id="5623e-121">3D</span><span class="sxs-lookup"><span data-stu-id="5623e-121">3</span></span>|<span data-ttu-id="5623e-122">Falha na última sincronização.</span><span class="sxs-lookup"><span data-stu-id="5623e-122">Last Sync failed.</span></span>|



