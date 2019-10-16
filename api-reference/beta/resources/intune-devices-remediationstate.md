---
title: tipo de enumeração remediable
description: Indica o tipo de status de execução do script de gerenciamento de dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b359842d7fb266803fdb758d32ca51e6a4b78b97
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37529085"
---
# <a name="remediationstate-enum-type"></a><span data-ttu-id="c4164-103">tipo de enumeração remediable</span><span class="sxs-lookup"><span data-stu-id="c4164-103">remediationState enum type</span></span>

> <span data-ttu-id="c4164-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c4164-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4164-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c4164-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4164-106">Indica o tipo de status de execução do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c4164-106">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="c4164-107">Membros</span><span class="sxs-lookup"><span data-stu-id="c4164-107">Members</span></span>
|<span data-ttu-id="c4164-108">Membro</span><span class="sxs-lookup"><span data-stu-id="c4164-108">Member</span></span>|<span data-ttu-id="c4164-109">Valor</span><span class="sxs-lookup"><span data-stu-id="c4164-109">Value</span></span>|<span data-ttu-id="c4164-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4164-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4164-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="c4164-111">unknown</span></span>|<span data-ttu-id="c4164-112">,0</span><span class="sxs-lookup"><span data-stu-id="c4164-112">0</span></span>|<span data-ttu-id="c4164-113">Resultado desconhecido.</span><span class="sxs-lookup"><span data-stu-id="c4164-113">Unknown result.</span></span>|
|<span data-ttu-id="c4164-114">ignorados</span><span class="sxs-lookup"><span data-stu-id="c4164-114">skipped</span></span>|<span data-ttu-id="c4164-115">1</span><span class="sxs-lookup"><span data-stu-id="c4164-115">1</span></span>|<span data-ttu-id="c4164-116">A execução do script de correção foi ignorada</span><span class="sxs-lookup"><span data-stu-id="c4164-116">Remediation script execution was skipped</span></span>|
|<span data-ttu-id="c4164-117">sucesso</span><span class="sxs-lookup"><span data-stu-id="c4164-117">success</span></span>|<span data-ttu-id="c4164-118">duas</span><span class="sxs-lookup"><span data-stu-id="c4164-118">2</span></span>|<span data-ttu-id="c4164-119">O script de correção foi executado com êxito e corrigiu o estado do dispositivo</span><span class="sxs-lookup"><span data-stu-id="c4164-119">Remediation script executed successfully and remediated the device state</span></span>|
|<span data-ttu-id="c4164-120">remediationFailed</span><span class="sxs-lookup"><span data-stu-id="c4164-120">remediationFailed</span></span>|<span data-ttu-id="c4164-121">3D</span><span class="sxs-lookup"><span data-stu-id="c4164-121">3</span></span>|<span data-ttu-id="c4164-122">O script de correção foi executado com êxito, mas falhou ao corrigir o estado do dispositivo</span><span class="sxs-lookup"><span data-stu-id="c4164-122">Remediation script executed successfully but failed to remediated the device state</span></span>|
|<span data-ttu-id="c4164-123">scriptError</span><span class="sxs-lookup"><span data-stu-id="c4164-123">scriptError</span></span>|<span data-ttu-id="c4164-124">4 </span><span class="sxs-lookup"><span data-stu-id="c4164-124">4</span></span>|<span data-ttu-id="c4164-125">Execução de script de correção encontrada e erro ou tempo limite esgotado</span><span class="sxs-lookup"><span data-stu-id="c4164-125">Remediation script execution encountered and error or timed out</span></span>|



