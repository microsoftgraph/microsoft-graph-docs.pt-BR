---
title: tipo de enumeração appLogUploadState
description: AppLogUploadStatus
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c6a0c880fe8fa7fe743bea3ad42fee6d1e24d209
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943113"
---
# <a name="apploguploadstate-enum-type"></a><span data-ttu-id="8deec-103">tipo de enumeração appLogUploadState</span><span class="sxs-lookup"><span data-stu-id="8deec-103">appLogUploadState enum type</span></span>

> <span data-ttu-id="8deec-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8deec-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8deec-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8deec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8deec-106">AppLogUploadStatus</span><span class="sxs-lookup"><span data-stu-id="8deec-106">AppLogUploadStatus</span></span>

## <a name="members"></a><span data-ttu-id="8deec-107">Membros</span><span class="sxs-lookup"><span data-stu-id="8deec-107">Members</span></span>
|<span data-ttu-id="8deec-108">Membro</span><span class="sxs-lookup"><span data-stu-id="8deec-108">Member</span></span>|<span data-ttu-id="8deec-109">Valor</span><span class="sxs-lookup"><span data-stu-id="8deec-109">Value</span></span>|<span data-ttu-id="8deec-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8deec-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8deec-111">função</span><span class="sxs-lookup"><span data-stu-id="8deec-111">pending</span></span>|<span data-ttu-id="8deec-112">,0</span><span class="sxs-lookup"><span data-stu-id="8deec-112">0</span></span>|<span data-ttu-id="8deec-113">A solicitação está aguardando processamento ou sob processamento</span><span class="sxs-lookup"><span data-stu-id="8deec-113">Request is waiting to be processed or under processing</span></span>|
|<span data-ttu-id="8deec-114">Completed</span><span class="sxs-lookup"><span data-stu-id="8deec-114">completed</span></span>|<span data-ttu-id="8deec-115">1</span><span class="sxs-lookup"><span data-stu-id="8deec-115">1</span></span>|<span data-ttu-id="8deec-116">A solicitação foi concluída com o arquivo carregado no blob do Azure para download.</span><span class="sxs-lookup"><span data-stu-id="8deec-116">Request is completed with file uploaded to Azure blob for download.</span></span>|
|<span data-ttu-id="8deec-117">falhou</span><span class="sxs-lookup"><span data-stu-id="8deec-117">failed</span></span>|<span data-ttu-id="8deec-118">duas</span><span class="sxs-lookup"><span data-stu-id="8deec-118">2</span></span>|<span data-ttu-id="8deec-119">Solicitar processamento concluído e em estado de erro.</span><span class="sxs-lookup"><span data-stu-id="8deec-119">Request finished processing and in error state.</span></span>|




