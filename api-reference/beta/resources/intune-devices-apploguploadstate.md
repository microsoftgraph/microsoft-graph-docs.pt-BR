---
title: tipo de enumeração appLogUploadState
description: AppLogUploadStatus
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: fed773a22ba0e538785211ece7849669efd9d383
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725523"
---
# <a name="apploguploadstate-enum-type"></a><span data-ttu-id="780ac-103">tipo de enumeração appLogUploadState</span><span class="sxs-lookup"><span data-stu-id="780ac-103">appLogUploadState enum type</span></span>

<span data-ttu-id="780ac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="780ac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="780ac-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="780ac-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="780ac-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="780ac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="780ac-107">AppLogUploadStatus</span><span class="sxs-lookup"><span data-stu-id="780ac-107">AppLogUploadStatus</span></span>

## <a name="members"></a><span data-ttu-id="780ac-108">Membros</span><span class="sxs-lookup"><span data-stu-id="780ac-108">Members</span></span>
|<span data-ttu-id="780ac-109">Membro</span><span class="sxs-lookup"><span data-stu-id="780ac-109">Member</span></span>|<span data-ttu-id="780ac-110">Valor</span><span class="sxs-lookup"><span data-stu-id="780ac-110">Value</span></span>|<span data-ttu-id="780ac-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="780ac-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="780ac-112">função</span><span class="sxs-lookup"><span data-stu-id="780ac-112">pending</span></span>|<span data-ttu-id="780ac-113">,0</span><span class="sxs-lookup"><span data-stu-id="780ac-113">0</span></span>|<span data-ttu-id="780ac-114">A solicitação está aguardando processamento ou sob processamento</span><span class="sxs-lookup"><span data-stu-id="780ac-114">Request is waiting to be processed or under processing</span></span>|
|<span data-ttu-id="780ac-115">Completed</span><span class="sxs-lookup"><span data-stu-id="780ac-115">completed</span></span>|<span data-ttu-id="780ac-116">1</span><span class="sxs-lookup"><span data-stu-id="780ac-116">1</span></span>|<span data-ttu-id="780ac-117">A solicitação foi concluída com o arquivo carregado no blob do Azure para download.</span><span class="sxs-lookup"><span data-stu-id="780ac-117">Request is completed with file uploaded to Azure blob for download.</span></span>|
|<span data-ttu-id="780ac-118">falhou</span><span class="sxs-lookup"><span data-stu-id="780ac-118">failed</span></span>|<span data-ttu-id="780ac-119">duas</span><span class="sxs-lookup"><span data-stu-id="780ac-119">2</span></span>|<span data-ttu-id="780ac-120">Solicitar processamento concluído e em estado de erro.</span><span class="sxs-lookup"><span data-stu-id="780ac-120">Request finished processing and in error state.</span></span>|





