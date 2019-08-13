---
title: tipo de enumeração runState
description: Indica o tipo de status de execução do script de gerenciamento de dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d77f3ef9a2d7fd37edeaf2b4cc25d5e6d5bfcf4f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347847"
---
# <a name="runstate-enum-type"></a><span data-ttu-id="3b547-103">tipo de enumeração runState</span><span class="sxs-lookup"><span data-stu-id="3b547-103">runState enum type</span></span>

> <span data-ttu-id="3b547-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3b547-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b547-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3b547-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b547-106">Indica o tipo de status de execução do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="3b547-106">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="3b547-107">Membros</span><span class="sxs-lookup"><span data-stu-id="3b547-107">Members</span></span>
|<span data-ttu-id="3b547-108">Membro</span><span class="sxs-lookup"><span data-stu-id="3b547-108">Member</span></span>|<span data-ttu-id="3b547-109">Valor</span><span class="sxs-lookup"><span data-stu-id="3b547-109">Value</span></span>|<span data-ttu-id="3b547-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b547-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b547-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="3b547-111">unknown</span></span>|<span data-ttu-id="3b547-112">,0</span><span class="sxs-lookup"><span data-stu-id="3b547-112">0</span></span>|<span data-ttu-id="3b547-113">Resultado desconhecido.</span><span class="sxs-lookup"><span data-stu-id="3b547-113">Unknown result.</span></span>|
|<span data-ttu-id="3b547-114">sucesso</span><span class="sxs-lookup"><span data-stu-id="3b547-114">success</span></span>|<span data-ttu-id="3b547-115">1</span><span class="sxs-lookup"><span data-stu-id="3b547-115">1</span></span>|<span data-ttu-id="3b547-116">O script é executado com êxito.</span><span class="sxs-lookup"><span data-stu-id="3b547-116">Script is run successfully.</span></span>|
|<span data-ttu-id="3b547-117">fail</span><span class="sxs-lookup"><span data-stu-id="3b547-117">fail</span></span>|<span data-ttu-id="3b547-118">duas</span><span class="sxs-lookup"><span data-stu-id="3b547-118">2</span></span>|<span data-ttu-id="3b547-119">O script não pôde ser executado.</span><span class="sxs-lookup"><span data-stu-id="3b547-119">Script failed to run.</span></span>|
|<span data-ttu-id="3b547-120">erro</span><span class="sxs-lookup"><span data-stu-id="3b547-120">error</span></span>|<span data-ttu-id="3b547-121">3D</span><span class="sxs-lookup"><span data-stu-id="3b547-121">3</span></span>|<span data-ttu-id="3b547-122">Erro de ocorrências de script de descoberta.</span><span class="sxs-lookup"><span data-stu-id="3b547-122">Discovery script hits error.</span></span>|
|<span data-ttu-id="3b547-123">função</span><span class="sxs-lookup"><span data-stu-id="3b547-123">pending</span></span>|<span data-ttu-id="3b547-124">quatro</span><span class="sxs-lookup"><span data-stu-id="3b547-124">4</span></span>|<span data-ttu-id="3b547-125">O script está pendente para execução.</span><span class="sxs-lookup"><span data-stu-id="3b547-125">Script is pending to execute.</span></span>|



