---
title: tipo de enumeração remediable
description: Indica o tipo de status de execução do script de gerenciamento de dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 90e930d6b8955671abb494839bafe6cac16438f0
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49230874"
---
# <a name="remediationstate-enum-type"></a><span data-ttu-id="f994d-103">tipo de enumeração remediable</span><span class="sxs-lookup"><span data-stu-id="f994d-103">remediationState enum type</span></span>

<span data-ttu-id="f994d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f994d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f994d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f994d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f994d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f994d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f994d-107">Indica o tipo de status de execução do script de gerenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f994d-107">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="f994d-108">Membros</span><span class="sxs-lookup"><span data-stu-id="f994d-108">Members</span></span>
|<span data-ttu-id="f994d-109">Membro</span><span class="sxs-lookup"><span data-stu-id="f994d-109">Member</span></span>|<span data-ttu-id="f994d-110">Valor</span><span class="sxs-lookup"><span data-stu-id="f994d-110">Value</span></span>|<span data-ttu-id="f994d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f994d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f994d-112">desconhecido</span><span class="sxs-lookup"><span data-stu-id="f994d-112">unknown</span></span>|<span data-ttu-id="f994d-113">,0</span><span class="sxs-lookup"><span data-stu-id="f994d-113">0</span></span>|<span data-ttu-id="f994d-114">Resultado desconhecido.</span><span class="sxs-lookup"><span data-stu-id="f994d-114">Unknown result.</span></span>|
|<span data-ttu-id="f994d-115">ignorados</span><span class="sxs-lookup"><span data-stu-id="f994d-115">skipped</span></span>|<span data-ttu-id="f994d-116">1</span><span class="sxs-lookup"><span data-stu-id="f994d-116">1</span></span>|<span data-ttu-id="f994d-117">A execução do script de correção foi ignorada</span><span class="sxs-lookup"><span data-stu-id="f994d-117">Remediation script execution was skipped</span></span>|
|<span data-ttu-id="f994d-118">sucesso</span><span class="sxs-lookup"><span data-stu-id="f994d-118">success</span></span>|<span data-ttu-id="f994d-119">duas</span><span class="sxs-lookup"><span data-stu-id="f994d-119">2</span></span>|<span data-ttu-id="f994d-120">O script de correção foi executado com êxito e corrigiu o estado do dispositivo</span><span class="sxs-lookup"><span data-stu-id="f994d-120">Remediation script executed successfully and remediated the device state</span></span>|
|<span data-ttu-id="f994d-121">remediationFailed</span><span class="sxs-lookup"><span data-stu-id="f994d-121">remediationFailed</span></span>|<span data-ttu-id="f994d-122">3D</span><span class="sxs-lookup"><span data-stu-id="f994d-122">3</span></span>|<span data-ttu-id="f994d-123">O script de correção foi executado com êxito, mas falhou ao corrigir o estado do dispositivo</span><span class="sxs-lookup"><span data-stu-id="f994d-123">Remediation script executed successfully but failed to remediated the device state</span></span>|
|<span data-ttu-id="f994d-124">scriptError</span><span class="sxs-lookup"><span data-stu-id="f994d-124">scriptError</span></span>|<span data-ttu-id="f994d-125">4 </span><span class="sxs-lookup"><span data-stu-id="f994d-125">4</span></span>|<span data-ttu-id="f994d-126">Execução de script de correção encontrada e erro ou tempo limite esgotado</span><span class="sxs-lookup"><span data-stu-id="f994d-126">Remediation script execution encountered and error or timed out</span></span>|




