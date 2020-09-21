---
title: tipo de enumeração edgeTelemetryMode
description: Tipo de dados de navegação enviados para a análise do Microsoft 365
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5ceb31c9a82fe2d13668aaf5db32b65beba88f26
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016265"
---
# <a name="edgetelemetrymode-enum-type"></a><span data-ttu-id="4dc57-103">tipo de enumeração edgeTelemetryMode</span><span class="sxs-lookup"><span data-stu-id="4dc57-103">edgeTelemetryMode enum type</span></span>

<span data-ttu-id="4dc57-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4dc57-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4dc57-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4dc57-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4dc57-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4dc57-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4dc57-107">Tipo de dados de navegação enviados para a análise do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="4dc57-107">Type of browsing data sent to Microsoft 365 analytics</span></span>

## <a name="members"></a><span data-ttu-id="4dc57-108">Membros</span><span class="sxs-lookup"><span data-stu-id="4dc57-108">Members</span></span>
|<span data-ttu-id="4dc57-109">Membro</span><span class="sxs-lookup"><span data-stu-id="4dc57-109">Member</span></span>|<span data-ttu-id="4dc57-110">Valor</span><span class="sxs-lookup"><span data-stu-id="4dc57-110">Value</span></span>|<span data-ttu-id="4dc57-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4dc57-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4dc57-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="4dc57-112">notConfigured</span></span>|<span data-ttu-id="4dc57-113">,0</span><span class="sxs-lookup"><span data-stu-id="4dc57-113">0</span></span>|<span data-ttu-id="4dc57-114">Padrão – nenhum dado de telemetria coletado ou enviado</span><span class="sxs-lookup"><span data-stu-id="4dc57-114">Default – No telemetry data collected or sent</span></span>|
|<span data-ttu-id="4dc57-115">Internet</span><span class="sxs-lookup"><span data-stu-id="4dc57-115">intranet</span></span>|<span data-ttu-id="4dc57-116">1 </span><span class="sxs-lookup"><span data-stu-id="4dc57-116">1</span></span>|<span data-ttu-id="4dc57-117">Permitir o envio de histórico de intranet somente: enviar apenas dados de histórico de navegação para sites de intranet</span><span class="sxs-lookup"><span data-stu-id="4dc57-117">Allow sending intranet history only: Only send browsing history data for intranet sites</span></span>|
|<span data-ttu-id="4dc57-118">provedor</span><span class="sxs-lookup"><span data-stu-id="4dc57-118">internet</span></span>|<span data-ttu-id="4dc57-119">2 </span><span class="sxs-lookup"><span data-stu-id="4dc57-119">2</span></span>|<span data-ttu-id="4dc57-120">Permitir o envio somente do histórico da Internet: Enviar somente dados de histórico de navegação para sites da Internet</span><span class="sxs-lookup"><span data-stu-id="4dc57-120">Allow sending internet history only: Only send browsing history data for internet sites</span></span>|
|<span data-ttu-id="4dc57-121">intranetAndInternet</span><span class="sxs-lookup"><span data-stu-id="4dc57-121">intranetAndInternet</span></span>|<span data-ttu-id="4dc57-122">3 </span><span class="sxs-lookup"><span data-stu-id="4dc57-122">3</span></span>|<span data-ttu-id="4dc57-123">Permitir o envio do histórico de intranet e Internet: enviar dados de histórico de navegação para sites de intranet e Internet</span><span class="sxs-lookup"><span data-stu-id="4dc57-123">Allow sending both intranet and internet history: Send browsing history data for intranet and internet sites</span></span>|






