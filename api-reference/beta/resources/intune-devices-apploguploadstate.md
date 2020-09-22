---
title: tipo de enumeração appLogUploadState
description: AppLogUploadStatus
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f3a39e8155c6cb18291ee233574c592f3ce964ca
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060830"
---
# <a name="apploguploadstate-enum-type"></a><span data-ttu-id="f3a83-103">tipo de enumeração appLogUploadState</span><span class="sxs-lookup"><span data-stu-id="f3a83-103">appLogUploadState enum type</span></span>

<span data-ttu-id="f3a83-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3a83-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f3a83-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f3a83-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3a83-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f3a83-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3a83-107">AppLogUploadStatus</span><span class="sxs-lookup"><span data-stu-id="f3a83-107">AppLogUploadStatus</span></span>

## <a name="members"></a><span data-ttu-id="f3a83-108">Membros</span><span class="sxs-lookup"><span data-stu-id="f3a83-108">Members</span></span>
|<span data-ttu-id="f3a83-109">Membro</span><span class="sxs-lookup"><span data-stu-id="f3a83-109">Member</span></span>|<span data-ttu-id="f3a83-110">Valor</span><span class="sxs-lookup"><span data-stu-id="f3a83-110">Value</span></span>|<span data-ttu-id="f3a83-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3a83-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3a83-112">função</span><span class="sxs-lookup"><span data-stu-id="f3a83-112">pending</span></span>|<span data-ttu-id="f3a83-113">,0</span><span class="sxs-lookup"><span data-stu-id="f3a83-113">0</span></span>|<span data-ttu-id="f3a83-114">A solicitação está aguardando processamento ou sob processamento</span><span class="sxs-lookup"><span data-stu-id="f3a83-114">Request is waiting to be processed or under processing</span></span>|
|<span data-ttu-id="f3a83-115">Completed</span><span class="sxs-lookup"><span data-stu-id="f3a83-115">completed</span></span>|<span data-ttu-id="f3a83-116">1 </span><span class="sxs-lookup"><span data-stu-id="f3a83-116">1</span></span>|<span data-ttu-id="f3a83-117">A solicitação foi concluída com o arquivo carregado no blob do Azure para download.</span><span class="sxs-lookup"><span data-stu-id="f3a83-117">Request is completed with file uploaded to Azure blob for download.</span></span>|
|<span data-ttu-id="f3a83-118">falhou</span><span class="sxs-lookup"><span data-stu-id="f3a83-118">failed</span></span>|<span data-ttu-id="f3a83-119">2 </span><span class="sxs-lookup"><span data-stu-id="f3a83-119">2</span></span>|<span data-ttu-id="f3a83-120">Solicitar processamento concluído e em estado de erro.</span><span class="sxs-lookup"><span data-stu-id="f3a83-120">Request finished processing and in error state.</span></span>|






