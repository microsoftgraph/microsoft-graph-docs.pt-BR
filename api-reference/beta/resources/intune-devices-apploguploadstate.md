---
title: tipo de enumeração appLogUploadState
description: AppLogUploadStatus
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d692e352f177c7f882a33e49604934c4b1a22912
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525163"
---
# <a name="apploguploadstate-enum-type"></a><span data-ttu-id="7262d-103">tipo de enumeração appLogUploadState</span><span class="sxs-lookup"><span data-stu-id="7262d-103">appLogUploadState enum type</span></span>

<span data-ttu-id="7262d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7262d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7262d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7262d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7262d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7262d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7262d-107">AppLogUploadStatus</span><span class="sxs-lookup"><span data-stu-id="7262d-107">AppLogUploadStatus</span></span>

## <a name="members"></a><span data-ttu-id="7262d-108">Membros</span><span class="sxs-lookup"><span data-stu-id="7262d-108">Members</span></span>
|<span data-ttu-id="7262d-109">Membro</span><span class="sxs-lookup"><span data-stu-id="7262d-109">Member</span></span>|<span data-ttu-id="7262d-110">Valor</span><span class="sxs-lookup"><span data-stu-id="7262d-110">Value</span></span>|<span data-ttu-id="7262d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7262d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7262d-112">função</span><span class="sxs-lookup"><span data-stu-id="7262d-112">pending</span></span>|<span data-ttu-id="7262d-113">,0</span><span class="sxs-lookup"><span data-stu-id="7262d-113">0</span></span>|<span data-ttu-id="7262d-114">A solicitação está aguardando processamento ou sob processamento</span><span class="sxs-lookup"><span data-stu-id="7262d-114">Request is waiting to be processed or under processing</span></span>|
|<span data-ttu-id="7262d-115">Completed</span><span class="sxs-lookup"><span data-stu-id="7262d-115">completed</span></span>|<span data-ttu-id="7262d-116">1 </span><span class="sxs-lookup"><span data-stu-id="7262d-116">1</span></span>|<span data-ttu-id="7262d-117">A solicitação foi concluída com o arquivo carregado no blob do Azure para download.</span><span class="sxs-lookup"><span data-stu-id="7262d-117">Request is completed with file uploaded to Azure blob for download.</span></span>|
|<span data-ttu-id="7262d-118">falhou</span><span class="sxs-lookup"><span data-stu-id="7262d-118">failed</span></span>|<span data-ttu-id="7262d-119">2 </span><span class="sxs-lookup"><span data-stu-id="7262d-119">2</span></span>|<span data-ttu-id="7262d-120">Solicitar processamento concluído e em estado de erro.</span><span class="sxs-lookup"><span data-stu-id="7262d-120">Request finished processing and in error state.</span></span>|



