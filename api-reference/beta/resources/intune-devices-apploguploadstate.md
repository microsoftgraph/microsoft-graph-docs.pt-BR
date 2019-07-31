---
title: tipo de enumeração appLogUploadState
description: AppLogUploadStatus
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ea94f8f8803c268c83d9c6419ad7128339e6d4cb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000001"
---
# <a name="apploguploadstate-enum-type"></a><span data-ttu-id="a6213-103">tipo de enumeração appLogUploadState</span><span class="sxs-lookup"><span data-stu-id="a6213-103">appLogUploadState enum type</span></span>

> <span data-ttu-id="a6213-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a6213-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6213-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a6213-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6213-106">AppLogUploadStatus</span><span class="sxs-lookup"><span data-stu-id="a6213-106">AppLogUploadStatus</span></span>

## <a name="members"></a><span data-ttu-id="a6213-107">Membros</span><span class="sxs-lookup"><span data-stu-id="a6213-107">Members</span></span>
|<span data-ttu-id="a6213-108">Membro</span><span class="sxs-lookup"><span data-stu-id="a6213-108">Member</span></span>|<span data-ttu-id="a6213-109">Valor</span><span class="sxs-lookup"><span data-stu-id="a6213-109">Value</span></span>|<span data-ttu-id="a6213-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6213-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6213-111">função</span><span class="sxs-lookup"><span data-stu-id="a6213-111">pending</span></span>|<span data-ttu-id="a6213-112">,0</span><span class="sxs-lookup"><span data-stu-id="a6213-112">0</span></span>|<span data-ttu-id="a6213-113">A solicitação está aguardando processamento ou sob processamento</span><span class="sxs-lookup"><span data-stu-id="a6213-113">Request is waiting to be processed or under processing</span></span>|
|<span data-ttu-id="a6213-114">Completed</span><span class="sxs-lookup"><span data-stu-id="a6213-114">completed</span></span>|<span data-ttu-id="a6213-115">1</span><span class="sxs-lookup"><span data-stu-id="a6213-115">1</span></span>|<span data-ttu-id="a6213-116">A solicitação foi concluída com o arquivo carregado no blob do Azure para download.</span><span class="sxs-lookup"><span data-stu-id="a6213-116">Request is completed with file uploaded to Azure blob for download.</span></span>|
|<span data-ttu-id="a6213-117">falhou</span><span class="sxs-lookup"><span data-stu-id="a6213-117">failed</span></span>|<span data-ttu-id="a6213-118">duas</span><span class="sxs-lookup"><span data-stu-id="a6213-118">2</span></span>|<span data-ttu-id="a6213-119">Solicitar processamento concluído e em estado de erro.</span><span class="sxs-lookup"><span data-stu-id="a6213-119">Request finished processing and in error state.</span></span>|





