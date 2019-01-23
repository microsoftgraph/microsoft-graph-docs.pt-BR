---
title: tipo de enum appLogUploadState
description: AppLogUploadStatus
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 58dcc0d4a15370d6449772d917e8994f0eb9e7bd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431306"
---
# <a name="apploguploadstate-enum-type"></a><span data-ttu-id="6c001-103">tipo de enum appLogUploadState</span><span class="sxs-lookup"><span data-stu-id="6c001-103">appLogUploadState enum type</span></span>

> <span data-ttu-id="6c001-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="6c001-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6c001-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6c001-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6c001-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="6c001-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c001-107">AppLogUploadStatus</span><span class="sxs-lookup"><span data-stu-id="6c001-107">AppLogUploadStatus</span></span>

## <a name="members"></a><span data-ttu-id="6c001-108">Membros</span><span class="sxs-lookup"><span data-stu-id="6c001-108">Members</span></span>
|<span data-ttu-id="6c001-109">Membro</span><span class="sxs-lookup"><span data-stu-id="6c001-109">Member</span></span>|<span data-ttu-id="6c001-110">Valor</span><span class="sxs-lookup"><span data-stu-id="6c001-110">Value</span></span>|<span data-ttu-id="6c001-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c001-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c001-112">pendente</span><span class="sxs-lookup"><span data-stu-id="6c001-112">pending</span></span>|<span data-ttu-id="6c001-113">0</span><span class="sxs-lookup"><span data-stu-id="6c001-113">0</span></span>|<span data-ttu-id="6c001-114">Solicitação está aguardando processamento ou em processamento</span><span class="sxs-lookup"><span data-stu-id="6c001-114">Request is waiting to be processed or under processing</span></span>|
|<span data-ttu-id="6c001-115">concluído</span><span class="sxs-lookup"><span data-stu-id="6c001-115">completed</span></span>|<span data-ttu-id="6c001-116">1</span><span class="sxs-lookup"><span data-stu-id="6c001-116">1</span></span>|<span data-ttu-id="6c001-117">Solicitação será preenchida com o arquivo carregado blob Azure para download.</span><span class="sxs-lookup"><span data-stu-id="6c001-117">Request is completed with file uploaded to Azure blob for download.</span></span>|
|<span data-ttu-id="6c001-118">Falha</span><span class="sxs-lookup"><span data-stu-id="6c001-118">failed</span></span>|<span data-ttu-id="6c001-119">2</span><span class="sxs-lookup"><span data-stu-id="6c001-119">2</span></span>|<span data-ttu-id="6c001-120">Concluir a solicitação de processamento e em estado de erro.</span><span class="sxs-lookup"><span data-stu-id="6c001-120">Request finished processing and in error state.</span></span>|




