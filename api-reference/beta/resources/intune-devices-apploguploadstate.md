---
title: tipo de enumeração appLogUploadState
description: AppLogUploadStatus
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 193344351f5654ea09c0246e06d1d3abf0d54039
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785130"
---
# <a name="apploguploadstate-enum-type"></a><span data-ttu-id="7f34f-103">tipo de enumeração appLogUploadState</span><span class="sxs-lookup"><span data-stu-id="7f34f-103">appLogUploadState enum type</span></span>

> <span data-ttu-id="7f34f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7f34f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f34f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7f34f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f34f-106">AppLogUploadStatus</span><span class="sxs-lookup"><span data-stu-id="7f34f-106">AppLogUploadStatus</span></span>

## <a name="members"></a><span data-ttu-id="7f34f-107">Membros</span><span class="sxs-lookup"><span data-stu-id="7f34f-107">Members</span></span>
|<span data-ttu-id="7f34f-108">Membro</span><span class="sxs-lookup"><span data-stu-id="7f34f-108">Member</span></span>|<span data-ttu-id="7f34f-109">Valor</span><span class="sxs-lookup"><span data-stu-id="7f34f-109">Value</span></span>|<span data-ttu-id="7f34f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f34f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f34f-111">função</span><span class="sxs-lookup"><span data-stu-id="7f34f-111">pending</span></span>|<span data-ttu-id="7f34f-112">,0</span><span class="sxs-lookup"><span data-stu-id="7f34f-112">0</span></span>|<span data-ttu-id="7f34f-113">A solicitação está aguardando processamento ou sob processamento</span><span class="sxs-lookup"><span data-stu-id="7f34f-113">Request is waiting to be processed or under processing</span></span>|
|<span data-ttu-id="7f34f-114">Completed</span><span class="sxs-lookup"><span data-stu-id="7f34f-114">completed</span></span>|<span data-ttu-id="7f34f-115">1</span><span class="sxs-lookup"><span data-stu-id="7f34f-115">1</span></span>|<span data-ttu-id="7f34f-116">A solicitação foi concluída com o arquivo carregado no blob do Azure para download.</span><span class="sxs-lookup"><span data-stu-id="7f34f-116">Request is completed with file uploaded to Azure blob for download.</span></span>|
|<span data-ttu-id="7f34f-117">falhou</span><span class="sxs-lookup"><span data-stu-id="7f34f-117">failed</span></span>|<span data-ttu-id="7f34f-118">duas</span><span class="sxs-lookup"><span data-stu-id="7f34f-118">2</span></span>|<span data-ttu-id="7f34f-119">Solicitar processamento concluído e em estado de erro.</span><span class="sxs-lookup"><span data-stu-id="7f34f-119">Request finished processing and in error state.</span></span>|



