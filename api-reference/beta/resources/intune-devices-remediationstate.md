---
title: tipo de enumeração remediable
description: Indica o tipo de status de execução do script de gerenciamento de dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: fb46c05ddbd1055f44794f0300077d47122aea25
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081115"
---
# <a name="remediationstate-enum-type"></a><span data-ttu-id="f17da-103">tipo de enumeração remediable</span><span class="sxs-lookup"><span data-stu-id="f17da-103">remediationState enum type</span></span>

<span data-ttu-id="f17da-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f17da-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f17da-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f17da-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f17da-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f17da-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f17da-107">Indica o tipo de status de execução do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f17da-107">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="f17da-108">Membros</span><span class="sxs-lookup"><span data-stu-id="f17da-108">Members</span></span>
|<span data-ttu-id="f17da-109">Membro</span><span class="sxs-lookup"><span data-stu-id="f17da-109">Member</span></span>|<span data-ttu-id="f17da-110">Valor</span><span class="sxs-lookup"><span data-stu-id="f17da-110">Value</span></span>|<span data-ttu-id="f17da-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f17da-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f17da-112">desconhecido</span><span class="sxs-lookup"><span data-stu-id="f17da-112">unknown</span></span>|<span data-ttu-id="f17da-113">,0</span><span class="sxs-lookup"><span data-stu-id="f17da-113">0</span></span>|<span data-ttu-id="f17da-114">Resultado desconhecido.</span><span class="sxs-lookup"><span data-stu-id="f17da-114">Unknown result.</span></span>|
|<span data-ttu-id="f17da-115">ignorados</span><span class="sxs-lookup"><span data-stu-id="f17da-115">skipped</span></span>|<span data-ttu-id="f17da-116">1 </span><span class="sxs-lookup"><span data-stu-id="f17da-116">1</span></span>|<span data-ttu-id="f17da-117">A execução do script de correção foi ignorada</span><span class="sxs-lookup"><span data-stu-id="f17da-117">Remediation script execution was skipped</span></span>|
|<span data-ttu-id="f17da-118">sucesso</span><span class="sxs-lookup"><span data-stu-id="f17da-118">success</span></span>|<span data-ttu-id="f17da-119">2 </span><span class="sxs-lookup"><span data-stu-id="f17da-119">2</span></span>|<span data-ttu-id="f17da-120">O script de correção foi executado com êxito e corrigiu o estado do dispositivo</span><span class="sxs-lookup"><span data-stu-id="f17da-120">Remediation script executed successfully and remediated the device state</span></span>|
|<span data-ttu-id="f17da-121">remediationFailed</span><span class="sxs-lookup"><span data-stu-id="f17da-121">remediationFailed</span></span>|<span data-ttu-id="f17da-122">3D</span><span class="sxs-lookup"><span data-stu-id="f17da-122">3</span></span>|<span data-ttu-id="f17da-123">O script de correção foi executado com êxito, mas falhou ao corrigir o estado do dispositivo</span><span class="sxs-lookup"><span data-stu-id="f17da-123">Remediation script executed successfully but failed to remediated the device state</span></span>|
|<span data-ttu-id="f17da-124">scriptError</span><span class="sxs-lookup"><span data-stu-id="f17da-124">scriptError</span></span>|<span data-ttu-id="f17da-125">4 </span><span class="sxs-lookup"><span data-stu-id="f17da-125">4</span></span>|<span data-ttu-id="f17da-126">Execução de script de correção encontrada e erro ou tempo limite esgotado</span><span class="sxs-lookup"><span data-stu-id="f17da-126">Remediation script execution encountered and error or timed out</span></span>|






