---
title: tipo de enumeração edgeTelemetryMode
description: Tipo de dados de navegação enviados para a análise do Microsoft 365
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d94fb93dcb7e95e0ba1ae7581ce5f26f44496002
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791832"
---
# <a name="edgetelemetrymode-enum-type"></a><span data-ttu-id="a1140-103">tipo de enumeração edgeTelemetryMode</span><span class="sxs-lookup"><span data-stu-id="a1140-103">edgeTelemetryMode enum type</span></span>

> <span data-ttu-id="a1140-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a1140-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1140-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a1140-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1140-106">Tipo de dados de navegação enviados para a análise do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="a1140-106">Type of browsing data sent to Microsoft 365 analytics</span></span>

## <a name="members"></a><span data-ttu-id="a1140-107">Membros</span><span class="sxs-lookup"><span data-stu-id="a1140-107">Members</span></span>
|<span data-ttu-id="a1140-108">Membro</span><span class="sxs-lookup"><span data-stu-id="a1140-108">Member</span></span>|<span data-ttu-id="a1140-109">Valor</span><span class="sxs-lookup"><span data-stu-id="a1140-109">Value</span></span>|<span data-ttu-id="a1140-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1140-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1140-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="a1140-111">notConfigured</span></span>|<span data-ttu-id="a1140-112">,0</span><span class="sxs-lookup"><span data-stu-id="a1140-112">0</span></span>|<span data-ttu-id="a1140-113">Padrão – nenhum dado de telemetria coletado ou enviado</span><span class="sxs-lookup"><span data-stu-id="a1140-113">Default – No telemetry data collected or sent</span></span>|
|<span data-ttu-id="a1140-114">Internet</span><span class="sxs-lookup"><span data-stu-id="a1140-114">intranet</span></span>|<span data-ttu-id="a1140-115">1</span><span class="sxs-lookup"><span data-stu-id="a1140-115">1</span></span>|<span data-ttu-id="a1140-116">Permitir o envio de histórico de intranet somente: enviar apenas dados de histórico de navegação para sites de intranet</span><span class="sxs-lookup"><span data-stu-id="a1140-116">Allow sending intranet history only: Only send browsing history data for intranet sites</span></span>|
|<span data-ttu-id="a1140-117">provedor</span><span class="sxs-lookup"><span data-stu-id="a1140-117">internet</span></span>|<span data-ttu-id="a1140-118">duas</span><span class="sxs-lookup"><span data-stu-id="a1140-118">2</span></span>|<span data-ttu-id="a1140-119">Permitir o envio somente do histórico da Internet: Enviar somente dados de histórico de navegação para sites da Internet</span><span class="sxs-lookup"><span data-stu-id="a1140-119">Allow sending internet history only: Only send browsing history data for internet sites</span></span>|
|<span data-ttu-id="a1140-120">intranetAndInternet</span><span class="sxs-lookup"><span data-stu-id="a1140-120">intranetAndInternet</span></span>|<span data-ttu-id="a1140-121">3D</span><span class="sxs-lookup"><span data-stu-id="a1140-121">3</span></span>|<span data-ttu-id="a1140-122">Permitir o envio do histórico de intranet e Internet: enviar dados de histórico de navegação para sites de intranet e Internet</span><span class="sxs-lookup"><span data-stu-id="a1140-122">Allow sending both intranet and internet history: Send browsing history data for intranet and internet sites</span></span>|



