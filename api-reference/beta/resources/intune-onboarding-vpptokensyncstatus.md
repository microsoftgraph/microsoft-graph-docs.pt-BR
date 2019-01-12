---
title: tipo de enum vppTokenSyncStatus
description: Status de sincronização possíveis associados com um token de programa de compra de Volume do Apple.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4101f1338513787b27ce530579ffd42c7756366a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931283"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="207c9-103">tipo de enum vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="207c9-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="207c9-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="207c9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="207c9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="207c9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="207c9-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="207c9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="207c9-107">Status de sincronização possíveis associados com um token de programa de compra de Volume do Apple.</span><span class="sxs-lookup"><span data-stu-id="207c9-107">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="207c9-108">Membros</span><span class="sxs-lookup"><span data-stu-id="207c9-108">Members</span></span>
|<span data-ttu-id="207c9-109">Membro</span><span class="sxs-lookup"><span data-stu-id="207c9-109">Member</span></span>|<span data-ttu-id="207c9-110">Valor</span><span class="sxs-lookup"><span data-stu-id="207c9-110">Value</span></span>|<span data-ttu-id="207c9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="207c9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="207c9-112">nenhum</span><span class="sxs-lookup"><span data-stu-id="207c9-112">none</span></span>|<span data-ttu-id="207c9-113">0</span><span class="sxs-lookup"><span data-stu-id="207c9-113">0</span></span>|<span data-ttu-id="207c9-114">Status do padrão.</span><span class="sxs-lookup"><span data-stu-id="207c9-114">Default status.</span></span>|
|<span data-ttu-id="207c9-115">inProgress</span><span class="sxs-lookup"><span data-stu-id="207c9-115">inProgress</span></span>|<span data-ttu-id="207c9-116">1</span><span class="sxs-lookup"><span data-stu-id="207c9-116">1</span></span>|<span data-ttu-id="207c9-117">Última sincronização em andamento.</span><span class="sxs-lookup"><span data-stu-id="207c9-117">Last Sync in progress.</span></span>|
|<span data-ttu-id="207c9-118">concluído</span><span class="sxs-lookup"><span data-stu-id="207c9-118">completed</span></span>|<span data-ttu-id="207c9-119">2</span><span class="sxs-lookup"><span data-stu-id="207c9-119">2</span></span>|<span data-ttu-id="207c9-120">Última sincronização concluída com êxito.</span><span class="sxs-lookup"><span data-stu-id="207c9-120">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="207c9-121">Falha</span><span class="sxs-lookup"><span data-stu-id="207c9-121">failed</span></span>|<span data-ttu-id="207c9-122">3</span><span class="sxs-lookup"><span data-stu-id="207c9-122">3</span></span>|<span data-ttu-id="207c9-123">Falha na última sincronização.</span><span class="sxs-lookup"><span data-stu-id="207c9-123">Last Sync failed.</span></span>|





