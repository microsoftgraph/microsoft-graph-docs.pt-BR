---
title: tipo de enum diagnosticDataSubmissionMode
description: Permitir que o dispositivo enviar dados de telemetria de diagnóstico e uso, como Watson.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: a293288c3891f8ecd77d422986e419d2e3d53767
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912943"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="1e4c7-103">tipo de enum diagnosticDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="1e4c7-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="1e4c7-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1e4c7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1e4c7-105">Permitir que o dispositivo enviar dados de telemetria de diagnóstico e uso, como Watson.</span><span class="sxs-lookup"><span data-stu-id="1e4c7-105">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>
## <a name="members"></a><span data-ttu-id="1e4c7-106">Membros</span><span class="sxs-lookup"><span data-stu-id="1e4c7-106">Members</span></span>
|<span data-ttu-id="1e4c7-107">Membro</span><span class="sxs-lookup"><span data-stu-id="1e4c7-107">Member</span></span>|<span data-ttu-id="1e4c7-108">Valor</span><span class="sxs-lookup"><span data-stu-id="1e4c7-108">Value</span></span>|<span data-ttu-id="1e4c7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e4c7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e4c7-110">userDefined</span><span class="sxs-lookup"><span data-stu-id="1e4c7-110">userDefined</span></span>|<span data-ttu-id="1e4c7-111">0</span><span class="sxs-lookup"><span data-stu-id="1e4c7-111">0</span></span>|<span data-ttu-id="1e4c7-112">Permitir que o usuário pode definir.</span><span class="sxs-lookup"><span data-stu-id="1e4c7-112">Allow the user to set.</span></span>|
|<span data-ttu-id="1e4c7-113">nenhum</span><span class="sxs-lookup"><span data-stu-id="1e4c7-113">none</span></span>|<span data-ttu-id="1e4c7-114">1</span><span class="sxs-lookup"><span data-stu-id="1e4c7-114">1</span></span>|<span data-ttu-id="1e4c7-115">Nenhum dado de telemetria é enviado de componentes do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="1e4c7-115">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="1e4c7-116">Observação: Esse valor só é aplicável aos dispositivos enterprise e servidor.</span><span class="sxs-lookup"><span data-stu-id="1e4c7-116">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="1e4c7-117">O uso dessa configuração em outros dispositivos é equivalente a definir o valor de 1.</span><span class="sxs-lookup"><span data-stu-id="1e4c7-117">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="1e4c7-118">básico</span><span class="sxs-lookup"><span data-stu-id="1e4c7-118">basic</span></span>|<span data-ttu-id="1e4c7-119">2</span><span class="sxs-lookup"><span data-stu-id="1e4c7-119">2</span></span>|<span data-ttu-id="1e4c7-120">Envia dados de Telemetria básica.</span><span class="sxs-lookup"><span data-stu-id="1e4c7-120">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="1e4c7-121">Avançado</span><span class="sxs-lookup"><span data-stu-id="1e4c7-121">enhanced</span></span>|<span data-ttu-id="1e4c7-122">3</span><span class="sxs-lookup"><span data-stu-id="1e4c7-122">3</span></span>|<span data-ttu-id="1e4c7-123">Envia aprimorado de dados de telemetria, incluindo dados de uso e ideias.</span><span class="sxs-lookup"><span data-stu-id="1e4c7-123">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="1e4c7-124">completo</span><span class="sxs-lookup"><span data-stu-id="1e4c7-124">full</span></span>|<span data-ttu-id="1e4c7-125">4</span><span class="sxs-lookup"><span data-stu-id="1e4c7-125">4</span></span>|<span data-ttu-id="1e4c7-126">Envia dados de telemetria completo incluindo dados de diagnósticos, como o estado do sistema.</span><span class="sxs-lookup"><span data-stu-id="1e4c7-126">Sends full telemetry data including diagnostic data, such as system state.</span></span>|



