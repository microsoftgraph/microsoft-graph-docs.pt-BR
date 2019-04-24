---
title: tipo de enumeração appLogUploadState
description: AppLogUploadStatus
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2b59210e7a00fde1e62e1cbc056f0bd34625330e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32467138"
---
# <a name="apploguploadstate-enum-type"></a><span data-ttu-id="752ed-103">tipo de enumeração appLogUploadState</span><span class="sxs-lookup"><span data-stu-id="752ed-103">appLogUploadState enum type</span></span>

> <span data-ttu-id="752ed-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="752ed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="752ed-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="752ed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="752ed-106">AppLogUploadStatus</span><span class="sxs-lookup"><span data-stu-id="752ed-106">AppLogUploadStatus</span></span>

## <a name="members"></a><span data-ttu-id="752ed-107">Membros</span><span class="sxs-lookup"><span data-stu-id="752ed-107">Members</span></span>
|<span data-ttu-id="752ed-108">Membro</span><span class="sxs-lookup"><span data-stu-id="752ed-108">Member</span></span>|<span data-ttu-id="752ed-109">Valor</span><span class="sxs-lookup"><span data-stu-id="752ed-109">Value</span></span>|<span data-ttu-id="752ed-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="752ed-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="752ed-111">função</span><span class="sxs-lookup"><span data-stu-id="752ed-111">pending</span></span>|<span data-ttu-id="752ed-112">,0</span><span class="sxs-lookup"><span data-stu-id="752ed-112">0</span></span>|<span data-ttu-id="752ed-113">A solicitação está aguardando processamento ou sob processamento</span><span class="sxs-lookup"><span data-stu-id="752ed-113">Request is waiting to be processed or under processing</span></span>|
|<span data-ttu-id="752ed-114">Completed</span><span class="sxs-lookup"><span data-stu-id="752ed-114">completed</span></span>|<span data-ttu-id="752ed-115">1</span><span class="sxs-lookup"><span data-stu-id="752ed-115">1</span></span>|<span data-ttu-id="752ed-116">A solicitação foi concluída com o arquivo carregado no blob do Azure para download.</span><span class="sxs-lookup"><span data-stu-id="752ed-116">Request is completed with file uploaded to Azure blob for download.</span></span>|
|<span data-ttu-id="752ed-117">falhou</span><span class="sxs-lookup"><span data-stu-id="752ed-117">failed</span></span>|<span data-ttu-id="752ed-118">duas</span><span class="sxs-lookup"><span data-stu-id="752ed-118">2</span></span>|<span data-ttu-id="752ed-119">Solicitar processamento concluído e em estado de erro.</span><span class="sxs-lookup"><span data-stu-id="752ed-119">Request finished processing and in error state.</span></span>|





