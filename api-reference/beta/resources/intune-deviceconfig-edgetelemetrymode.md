---
title: tipo de enumeração edgeTelemetryMode
description: Tipo de dados de navegação enviados para a análise do Microsoft 365
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 09cd5012d0b3a07a203b89ed76062232c47cfa82
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530030"
---
# <a name="edgetelemetrymode-enum-type"></a><span data-ttu-id="6babd-103">tipo de enumeração edgeTelemetryMode</span><span class="sxs-lookup"><span data-stu-id="6babd-103">edgeTelemetryMode enum type</span></span>

<span data-ttu-id="6babd-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6babd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6babd-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6babd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6babd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6babd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6babd-107">Tipo de dados de navegação enviados para a análise do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="6babd-107">Type of browsing data sent to Microsoft 365 analytics</span></span>

## <a name="members"></a><span data-ttu-id="6babd-108">Membros</span><span class="sxs-lookup"><span data-stu-id="6babd-108">Members</span></span>
|<span data-ttu-id="6babd-109">Membro</span><span class="sxs-lookup"><span data-stu-id="6babd-109">Member</span></span>|<span data-ttu-id="6babd-110">Valor</span><span class="sxs-lookup"><span data-stu-id="6babd-110">Value</span></span>|<span data-ttu-id="6babd-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6babd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6babd-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="6babd-112">notConfigured</span></span>|<span data-ttu-id="6babd-113">,0</span><span class="sxs-lookup"><span data-stu-id="6babd-113">0</span></span>|<span data-ttu-id="6babd-114">Padrão – nenhum dado de telemetria coletado ou enviado</span><span class="sxs-lookup"><span data-stu-id="6babd-114">Default – No telemetry data collected or sent</span></span>|
|<span data-ttu-id="6babd-115">Internet</span><span class="sxs-lookup"><span data-stu-id="6babd-115">intranet</span></span>|<span data-ttu-id="6babd-116">1 </span><span class="sxs-lookup"><span data-stu-id="6babd-116">1</span></span>|<span data-ttu-id="6babd-117">Permitir o envio de histórico de intranet somente: enviar apenas dados de histórico de navegação para sites de intranet</span><span class="sxs-lookup"><span data-stu-id="6babd-117">Allow sending intranet history only: Only send browsing history data for intranet sites</span></span>|
|<span data-ttu-id="6babd-118">provedor</span><span class="sxs-lookup"><span data-stu-id="6babd-118">internet</span></span>|<span data-ttu-id="6babd-119">2 </span><span class="sxs-lookup"><span data-stu-id="6babd-119">2</span></span>|<span data-ttu-id="6babd-120">Permitir o envio somente do histórico da Internet: Enviar somente dados de histórico de navegação para sites da Internet</span><span class="sxs-lookup"><span data-stu-id="6babd-120">Allow sending internet history only: Only send browsing history data for internet sites</span></span>|
|<span data-ttu-id="6babd-121">intranetAndInternet</span><span class="sxs-lookup"><span data-stu-id="6babd-121">intranetAndInternet</span></span>|<span data-ttu-id="6babd-122">3 </span><span class="sxs-lookup"><span data-stu-id="6babd-122">3</span></span>|<span data-ttu-id="6babd-123">Permitir o envio do histórico de intranet e Internet: enviar dados de histórico de navegação para sites de intranet e Internet</span><span class="sxs-lookup"><span data-stu-id="6babd-123">Allow sending both intranet and internet history: Send browsing history data for intranet and internet sites</span></span>|



