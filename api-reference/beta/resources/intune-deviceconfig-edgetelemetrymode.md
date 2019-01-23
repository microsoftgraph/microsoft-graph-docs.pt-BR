---
title: tipo de enum edgeTelemetryMode
description: Tipo de dados enviados à Microsoft 365 análise de navegação
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 81d429f7629a5d6a6f2593785605902065d9f1c7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429120"
---
# <a name="edgetelemetrymode-enum-type"></a><span data-ttu-id="30cde-103">tipo de enum edgeTelemetryMode</span><span class="sxs-lookup"><span data-stu-id="30cde-103">edgeTelemetryMode enum type</span></span>

> <span data-ttu-id="30cde-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="30cde-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="30cde-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="30cde-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="30cde-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="30cde-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30cde-107">Tipo de dados enviados à Microsoft 365 análise de navegação</span><span class="sxs-lookup"><span data-stu-id="30cde-107">Type of browsing data sent to Microsoft 365 analytics</span></span>

## <a name="members"></a><span data-ttu-id="30cde-108">Membros</span><span class="sxs-lookup"><span data-stu-id="30cde-108">Members</span></span>
|<span data-ttu-id="30cde-109">Membro</span><span class="sxs-lookup"><span data-stu-id="30cde-109">Member</span></span>|<span data-ttu-id="30cde-110">Valor</span><span class="sxs-lookup"><span data-stu-id="30cde-110">Value</span></span>|<span data-ttu-id="30cde-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="30cde-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30cde-112">não-configuradas</span><span class="sxs-lookup"><span data-stu-id="30cde-112">notConfigured</span></span>|<span data-ttu-id="30cde-113">0</span><span class="sxs-lookup"><span data-stu-id="30cde-113">0</span></span>|<span data-ttu-id="30cde-114">Padrão – sem dados de telemetria coletados ou enviados</span><span class="sxs-lookup"><span data-stu-id="30cde-114">Default – No telemetry data collected or sent</span></span>|
|<span data-ttu-id="30cde-115">intranet</span><span class="sxs-lookup"><span data-stu-id="30cde-115">intranet</span></span>|<span data-ttu-id="30cde-116">1</span><span class="sxs-lookup"><span data-stu-id="30cde-116">1</span></span>|<span data-ttu-id="30cde-117">Permitir envio somente histórico de intranet: somente enviar dados para sites de intranet do histórico de navegação</span><span class="sxs-lookup"><span data-stu-id="30cde-117">Allow sending intranet history only: Only send browsing history data for intranet sites</span></span>|
|<span data-ttu-id="30cde-118">Internet</span><span class="sxs-lookup"><span data-stu-id="30cde-118">internet</span></span>|<span data-ttu-id="30cde-119">2</span><span class="sxs-lookup"><span data-stu-id="30cde-119">2</span></span>|<span data-ttu-id="30cde-120">Permitem o envio somente histórico de internet: enviar apenas procurando dados de histórico para sites da internet</span><span class="sxs-lookup"><span data-stu-id="30cde-120">Allow sending internet history only: Only send browsing history data for internet sites</span></span>|
|<span data-ttu-id="30cde-121">intranetAndInternet</span><span class="sxs-lookup"><span data-stu-id="30cde-121">intranetAndInternet</span></span>|<span data-ttu-id="30cde-122">3</span><span class="sxs-lookup"><span data-stu-id="30cde-122">3</span></span>|<span data-ttu-id="30cde-123">Permitem o envio de histórico de intranet quanto da internet: envio procurando dados de histórico para sites de intranet e internet</span><span class="sxs-lookup"><span data-stu-id="30cde-123">Allow sending both intranet and internet history: Send browsing history data for intranet and internet sites</span></span>|




