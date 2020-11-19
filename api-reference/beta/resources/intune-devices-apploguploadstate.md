---
title: tipo de enumeração appLogUploadState
description: AppLogUploadStatus
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 2acf8fd19bcbadcbe6cb2371bf357babd4889b7b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49267842"
---
# <a name="apploguploadstate-enum-type"></a><span data-ttu-id="e3e5d-103">tipo de enumeração appLogUploadState</span><span class="sxs-lookup"><span data-stu-id="e3e5d-103">appLogUploadState enum type</span></span>

<span data-ttu-id="e3e5d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3e5d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e3e5d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e3e5d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3e5d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e3e5d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3e5d-107">AppLogUploadStatus</span><span class="sxs-lookup"><span data-stu-id="e3e5d-107">AppLogUploadStatus</span></span>

## <a name="members"></a><span data-ttu-id="e3e5d-108">Membros</span><span class="sxs-lookup"><span data-stu-id="e3e5d-108">Members</span></span>
|<span data-ttu-id="e3e5d-109">Membro</span><span class="sxs-lookup"><span data-stu-id="e3e5d-109">Member</span></span>|<span data-ttu-id="e3e5d-110">Valor</span><span class="sxs-lookup"><span data-stu-id="e3e5d-110">Value</span></span>|<span data-ttu-id="e3e5d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3e5d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3e5d-112">função</span><span class="sxs-lookup"><span data-stu-id="e3e5d-112">pending</span></span>|<span data-ttu-id="e3e5d-113">,0</span><span class="sxs-lookup"><span data-stu-id="e3e5d-113">0</span></span>|<span data-ttu-id="e3e5d-114">A solicitação está aguardando processamento ou sob processamento</span><span class="sxs-lookup"><span data-stu-id="e3e5d-114">Request is waiting to be processed or under processing</span></span>|
|<span data-ttu-id="e3e5d-115">Completed</span><span class="sxs-lookup"><span data-stu-id="e3e5d-115">completed</span></span>|<span data-ttu-id="e3e5d-116">1</span><span class="sxs-lookup"><span data-stu-id="e3e5d-116">1</span></span>|<span data-ttu-id="e3e5d-117">A solicitação foi concluída com o arquivo carregado no blob do Azure para download.</span><span class="sxs-lookup"><span data-stu-id="e3e5d-117">Request is completed with file uploaded to Azure blob for download.</span></span>|
|<span data-ttu-id="e3e5d-118">falhou</span><span class="sxs-lookup"><span data-stu-id="e3e5d-118">failed</span></span>|<span data-ttu-id="e3e5d-119">duas</span><span class="sxs-lookup"><span data-stu-id="e3e5d-119">2</span></span>|<span data-ttu-id="e3e5d-120">Solicitar processamento concluído e em estado de erro.</span><span class="sxs-lookup"><span data-stu-id="e3e5d-120">Request finished processing and in error state.</span></span>|




