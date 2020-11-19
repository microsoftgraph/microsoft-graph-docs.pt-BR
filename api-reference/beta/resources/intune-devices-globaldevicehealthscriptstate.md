---
title: tipo de enumeração globalDeviceHealthScriptState
description: Indica se os scripts de integridade do dispositivo global estão habilitados e em qual estado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7883fe642b4e7772caa6a13241db0b8e62d7fb98
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49299090"
---
# <a name="globaldevicehealthscriptstate-enum-type"></a><span data-ttu-id="307c9-103">tipo de enumeração globalDeviceHealthScriptState</span><span class="sxs-lookup"><span data-stu-id="307c9-103">globalDeviceHealthScriptState enum type</span></span>

<span data-ttu-id="307c9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="307c9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="307c9-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="307c9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="307c9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="307c9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="307c9-107">Indica se os scripts de integridade do dispositivo global estão habilitados e em qual estado</span><span class="sxs-lookup"><span data-stu-id="307c9-107">Indicates whether global device health scripts are enabled and are in which state</span></span>

## <a name="members"></a><span data-ttu-id="307c9-108">Membros</span><span class="sxs-lookup"><span data-stu-id="307c9-108">Members</span></span>
|<span data-ttu-id="307c9-109">Membro</span><span class="sxs-lookup"><span data-stu-id="307c9-109">Member</span></span>|<span data-ttu-id="307c9-110">Valor</span><span class="sxs-lookup"><span data-stu-id="307c9-110">Value</span></span>|<span data-ttu-id="307c9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="307c9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="307c9-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="307c9-112">notConfigured</span></span>|<span data-ttu-id="307c9-113">,0</span><span class="sxs-lookup"><span data-stu-id="307c9-113">0</span></span>|<span data-ttu-id="307c9-114">Os scripts de integridade do dispositivo global não estão configurados</span><span class="sxs-lookup"><span data-stu-id="307c9-114">Global device health scripts are not configured</span></span>|
|<span data-ttu-id="307c9-115">função</span><span class="sxs-lookup"><span data-stu-id="307c9-115">pending</span></span>|<span data-ttu-id="307c9-116">1</span><span class="sxs-lookup"><span data-stu-id="307c9-116">1</span></span>|<span data-ttu-id="307c9-117">Os scripts de integridade do dispositivo global estão configurados, mas não estão totalmente habilitados</span><span class="sxs-lookup"><span data-stu-id="307c9-117">Global device health scripts are configured but not fully enabled</span></span>|
|<span data-ttu-id="307c9-118">habilitadas</span><span class="sxs-lookup"><span data-stu-id="307c9-118">enabled</span></span>|<span data-ttu-id="307c9-119">duas</span><span class="sxs-lookup"><span data-stu-id="307c9-119">2</span></span>|<span data-ttu-id="307c9-120">Os scripts de integridade do dispositivo global estão habilitados e prontos para uso</span><span class="sxs-lookup"><span data-stu-id="307c9-120">Global device health scripts are enabled and ready to use</span></span>|




