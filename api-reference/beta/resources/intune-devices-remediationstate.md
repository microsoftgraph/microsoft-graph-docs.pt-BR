---
title: tipo de enumeração remediable
description: Indica o tipo de status de execução do script de gerenciamento de dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 49161209ad1a38123067ed3c434cbe31a3a2af70
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725425"
---
# <a name="remediationstate-enum-type"></a><span data-ttu-id="4c699-103">tipo de enumeração remediable</span><span class="sxs-lookup"><span data-stu-id="4c699-103">remediationState enum type</span></span>

<span data-ttu-id="4c699-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c699-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4c699-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4c699-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c699-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4c699-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c699-107">Indica o tipo de status de execução do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4c699-107">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="4c699-108">Membros</span><span class="sxs-lookup"><span data-stu-id="4c699-108">Members</span></span>
|<span data-ttu-id="4c699-109">Membro</span><span class="sxs-lookup"><span data-stu-id="4c699-109">Member</span></span>|<span data-ttu-id="4c699-110">Valor</span><span class="sxs-lookup"><span data-stu-id="4c699-110">Value</span></span>|<span data-ttu-id="4c699-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c699-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c699-112">desconhecido</span><span class="sxs-lookup"><span data-stu-id="4c699-112">unknown</span></span>|<span data-ttu-id="4c699-113">,0</span><span class="sxs-lookup"><span data-stu-id="4c699-113">0</span></span>|<span data-ttu-id="4c699-114">Resultado desconhecido.</span><span class="sxs-lookup"><span data-stu-id="4c699-114">Unknown result.</span></span>|
|<span data-ttu-id="4c699-115">ignorados</span><span class="sxs-lookup"><span data-stu-id="4c699-115">skipped</span></span>|<span data-ttu-id="4c699-116">1</span><span class="sxs-lookup"><span data-stu-id="4c699-116">1</span></span>|<span data-ttu-id="4c699-117">A execução do script de correção foi ignorada</span><span class="sxs-lookup"><span data-stu-id="4c699-117">Remediation script execution was skipped</span></span>|
|<span data-ttu-id="4c699-118">sucesso</span><span class="sxs-lookup"><span data-stu-id="4c699-118">success</span></span>|<span data-ttu-id="4c699-119">duas</span><span class="sxs-lookup"><span data-stu-id="4c699-119">2</span></span>|<span data-ttu-id="4c699-120">O script de correção foi executado com êxito e corrigiu o estado do dispositivo</span><span class="sxs-lookup"><span data-stu-id="4c699-120">Remediation script executed successfully and remediated the device state</span></span>|
|<span data-ttu-id="4c699-121">remediationFailed</span><span class="sxs-lookup"><span data-stu-id="4c699-121">remediationFailed</span></span>|<span data-ttu-id="4c699-122">3D</span><span class="sxs-lookup"><span data-stu-id="4c699-122">3</span></span>|<span data-ttu-id="4c699-123">O script de correção foi executado com êxito, mas falhou ao corrigir o estado do dispositivo</span><span class="sxs-lookup"><span data-stu-id="4c699-123">Remediation script executed successfully but failed to remediated the device state</span></span>|
|<span data-ttu-id="4c699-124">scriptError</span><span class="sxs-lookup"><span data-stu-id="4c699-124">scriptError</span></span>|<span data-ttu-id="4c699-125">4 </span><span class="sxs-lookup"><span data-stu-id="4c699-125">4</span></span>|<span data-ttu-id="4c699-126">Execução de script de correção encontrada e erro ou tempo limite esgotado</span><span class="sxs-lookup"><span data-stu-id="4c699-126">Remediation script execution encountered and error or timed out</span></span>|





