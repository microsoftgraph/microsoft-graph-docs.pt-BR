---
title: tipo de enumeração edgeTelemetryMode
description: Tipo de dados de navegação enviados para a análise do Microsoft 365
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1d671849e34d27403450ae6324b824a92ae9d9b4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566035"
---
# <a name="edgetelemetrymode-enum-type"></a><span data-ttu-id="11e7e-103">tipo de enumeração edgeTelemetryMode</span><span class="sxs-lookup"><span data-stu-id="11e7e-103">edgeTelemetryMode enum type</span></span>

> <span data-ttu-id="11e7e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="11e7e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11e7e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="11e7e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11e7e-106">Tipo de dados de navegação enviados para a análise do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="11e7e-106">Type of browsing data sent to Microsoft 365 analytics</span></span>

## <a name="members"></a><span data-ttu-id="11e7e-107">Membros</span><span class="sxs-lookup"><span data-stu-id="11e7e-107">Members</span></span>
|<span data-ttu-id="11e7e-108">Membro</span><span class="sxs-lookup"><span data-stu-id="11e7e-108">Member</span></span>|<span data-ttu-id="11e7e-109">Valor</span><span class="sxs-lookup"><span data-stu-id="11e7e-109">Value</span></span>|<span data-ttu-id="11e7e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="11e7e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11e7e-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="11e7e-111">notConfigured</span></span>|<span data-ttu-id="11e7e-112">,0</span><span class="sxs-lookup"><span data-stu-id="11e7e-112">0</span></span>|<span data-ttu-id="11e7e-113">Padrão – nenhum dado de telemetria coletado ou enviado</span><span class="sxs-lookup"><span data-stu-id="11e7e-113">Default – No telemetry data collected or sent</span></span>|
|<span data-ttu-id="11e7e-114">Internet</span><span class="sxs-lookup"><span data-stu-id="11e7e-114">intranet</span></span>|<span data-ttu-id="11e7e-115">1 </span><span class="sxs-lookup"><span data-stu-id="11e7e-115">1</span></span>|<span data-ttu-id="11e7e-116">Permitir o envio de histórico de intranet somente: enviar apenas dados de histórico de navegação para sites de intranet</span><span class="sxs-lookup"><span data-stu-id="11e7e-116">Allow sending intranet history only: Only send browsing history data for intranet sites</span></span>|
|<span data-ttu-id="11e7e-117">provedor</span><span class="sxs-lookup"><span data-stu-id="11e7e-117">internet</span></span>|<span data-ttu-id="11e7e-118">2 </span><span class="sxs-lookup"><span data-stu-id="11e7e-118">2</span></span>|<span data-ttu-id="11e7e-119">Permitir o envio somente do histórico da Internet: Enviar somente dados de histórico de navegação para sites da Internet</span><span class="sxs-lookup"><span data-stu-id="11e7e-119">Allow sending internet history only: Only send browsing history data for internet sites</span></span>|
|<span data-ttu-id="11e7e-120">intranetAndInternet</span><span class="sxs-lookup"><span data-stu-id="11e7e-120">intranetAndInternet</span></span>|<span data-ttu-id="11e7e-121">3 </span><span class="sxs-lookup"><span data-stu-id="11e7e-121">3</span></span>|<span data-ttu-id="11e7e-122">Permitir o envio do histórico de intranet e Internet: enviar dados de histórico de navegação para sites de intranet e Internet</span><span class="sxs-lookup"><span data-stu-id="11e7e-122">Allow sending both intranet and internet history: Send browsing history data for intranet and internet sites</span></span>|





