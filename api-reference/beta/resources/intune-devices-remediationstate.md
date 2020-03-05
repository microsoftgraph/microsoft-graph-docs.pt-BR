---
title: tipo de enumeração remediable
description: Indica o tipo de status de execução do script de gerenciamento de dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: dc2be0c860ba142f59bba05a2a0c5ae0105c0ab1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528511"
---
# <a name="remediationstate-enum-type"></a><span data-ttu-id="b3eb2-103">tipo de enumeração remediable</span><span class="sxs-lookup"><span data-stu-id="b3eb2-103">remediationState enum type</span></span>

<span data-ttu-id="b3eb2-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="b3eb2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b3eb2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b3eb2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3eb2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b3eb2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3eb2-107">Indica o tipo de status de execução do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b3eb2-107">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="b3eb2-108">Membros</span><span class="sxs-lookup"><span data-stu-id="b3eb2-108">Members</span></span>
|<span data-ttu-id="b3eb2-109">Membro</span><span class="sxs-lookup"><span data-stu-id="b3eb2-109">Member</span></span>|<span data-ttu-id="b3eb2-110">Valor</span><span class="sxs-lookup"><span data-stu-id="b3eb2-110">Value</span></span>|<span data-ttu-id="b3eb2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b3eb2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3eb2-112">desconhecido</span><span class="sxs-lookup"><span data-stu-id="b3eb2-112">unknown</span></span>|<span data-ttu-id="b3eb2-113">,0</span><span class="sxs-lookup"><span data-stu-id="b3eb2-113">0</span></span>|<span data-ttu-id="b3eb2-114">Resultado desconhecido.</span><span class="sxs-lookup"><span data-stu-id="b3eb2-114">Unknown result.</span></span>|
|<span data-ttu-id="b3eb2-115">ignorados</span><span class="sxs-lookup"><span data-stu-id="b3eb2-115">skipped</span></span>|<span data-ttu-id="b3eb2-116">1 </span><span class="sxs-lookup"><span data-stu-id="b3eb2-116">1</span></span>|<span data-ttu-id="b3eb2-117">A execução do script de correção foi ignorada</span><span class="sxs-lookup"><span data-stu-id="b3eb2-117">Remediation script execution was skipped</span></span>|
|<span data-ttu-id="b3eb2-118">sucesso</span><span class="sxs-lookup"><span data-stu-id="b3eb2-118">success</span></span>|<span data-ttu-id="b3eb2-119">2 </span><span class="sxs-lookup"><span data-stu-id="b3eb2-119">2</span></span>|<span data-ttu-id="b3eb2-120">O script de correção foi executado com êxito e corrigiu o estado do dispositivo</span><span class="sxs-lookup"><span data-stu-id="b3eb2-120">Remediation script executed successfully and remediated the device state</span></span>|
|<span data-ttu-id="b3eb2-121">remediationFailed</span><span class="sxs-lookup"><span data-stu-id="b3eb2-121">remediationFailed</span></span>|<span data-ttu-id="b3eb2-122">3 </span><span class="sxs-lookup"><span data-stu-id="b3eb2-122">3</span></span>|<span data-ttu-id="b3eb2-123">O script de correção foi executado com êxito, mas falhou ao corrigir o estado do dispositivo</span><span class="sxs-lookup"><span data-stu-id="b3eb2-123">Remediation script executed successfully but failed to remediated the device state</span></span>|
|<span data-ttu-id="b3eb2-124">scriptError</span><span class="sxs-lookup"><span data-stu-id="b3eb2-124">scriptError</span></span>|<span data-ttu-id="b3eb2-125">4 </span><span class="sxs-lookup"><span data-stu-id="b3eb2-125">4</span></span>|<span data-ttu-id="b3eb2-126">Execução de script de correção encontrada e erro ou tempo limite esgotado</span><span class="sxs-lookup"><span data-stu-id="b3eb2-126">Remediation script execution encountered and error or timed out</span></span>|



