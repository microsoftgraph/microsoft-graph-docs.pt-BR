---
title: tipo de enumeração edgeTelemetryMode
description: Tipo de dados de navegação enviados para a análise do Microsoft 365
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 87663359f015d2b0ae854715b4ed7fe09a7c1973
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728574"
---
# <a name="edgetelemetrymode-enum-type"></a><span data-ttu-id="cb5e2-103">tipo de enumeração edgeTelemetryMode</span><span class="sxs-lookup"><span data-stu-id="cb5e2-103">edgeTelemetryMode enum type</span></span>

<span data-ttu-id="cb5e2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb5e2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cb5e2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cb5e2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb5e2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cb5e2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb5e2-107">Tipo de dados de navegação enviados para a análise do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="cb5e2-107">Type of browsing data sent to Microsoft 365 analytics</span></span>

## <a name="members"></a><span data-ttu-id="cb5e2-108">Membros</span><span class="sxs-lookup"><span data-stu-id="cb5e2-108">Members</span></span>
|<span data-ttu-id="cb5e2-109">Membro</span><span class="sxs-lookup"><span data-stu-id="cb5e2-109">Member</span></span>|<span data-ttu-id="cb5e2-110">Valor</span><span class="sxs-lookup"><span data-stu-id="cb5e2-110">Value</span></span>|<span data-ttu-id="cb5e2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cb5e2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb5e2-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="cb5e2-112">notConfigured</span></span>|<span data-ttu-id="cb5e2-113">,0</span><span class="sxs-lookup"><span data-stu-id="cb5e2-113">0</span></span>|<span data-ttu-id="cb5e2-114">Padrão – nenhum dado de telemetria coletado ou enviado</span><span class="sxs-lookup"><span data-stu-id="cb5e2-114">Default – No telemetry data collected or sent</span></span>|
|<span data-ttu-id="cb5e2-115">Internet</span><span class="sxs-lookup"><span data-stu-id="cb5e2-115">intranet</span></span>|<span data-ttu-id="cb5e2-116">1</span><span class="sxs-lookup"><span data-stu-id="cb5e2-116">1</span></span>|<span data-ttu-id="cb5e2-117">Permitir o envio de histórico de intranet somente: enviar apenas dados de histórico de navegação para sites de intranet</span><span class="sxs-lookup"><span data-stu-id="cb5e2-117">Allow sending intranet history only: Only send browsing history data for intranet sites</span></span>|
|<span data-ttu-id="cb5e2-118">provedor</span><span class="sxs-lookup"><span data-stu-id="cb5e2-118">internet</span></span>|<span data-ttu-id="cb5e2-119">duas</span><span class="sxs-lookup"><span data-stu-id="cb5e2-119">2</span></span>|<span data-ttu-id="cb5e2-120">Permitir o envio somente do histórico da Internet: Enviar somente dados de histórico de navegação para sites da Internet</span><span class="sxs-lookup"><span data-stu-id="cb5e2-120">Allow sending internet history only: Only send browsing history data for internet sites</span></span>|
|<span data-ttu-id="cb5e2-121">intranetAndInternet</span><span class="sxs-lookup"><span data-stu-id="cb5e2-121">intranetAndInternet</span></span>|<span data-ttu-id="cb5e2-122">3D</span><span class="sxs-lookup"><span data-stu-id="cb5e2-122">3</span></span>|<span data-ttu-id="cb5e2-123">Permitir o envio do histórico de intranet e Internet: enviar dados de histórico de navegação para sites de intranet e Internet</span><span class="sxs-lookup"><span data-stu-id="cb5e2-123">Allow sending both intranet and internet history: Send browsing history data for intranet and internet sites</span></span>|





