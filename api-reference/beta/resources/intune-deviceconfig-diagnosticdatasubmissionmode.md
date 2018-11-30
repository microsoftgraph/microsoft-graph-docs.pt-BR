---
title: tipo de enum diagnosticDataSubmissionMode
description: Permitir que o dispositivo enviar dados de telemetria de diagnóstico e uso, como Watson.
ms.openlocfilehash: 9cdc76691df0a7a9492524d02c338ee2a42106e3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033968"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="6ec00-103">tipo de enum diagnosticDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="6ec00-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="6ec00-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6ec00-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6ec00-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6ec00-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6ec00-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6ec00-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6ec00-107">Permitir que o dispositivo enviar dados de telemetria de diagnóstico e uso, como Watson.</span><span class="sxs-lookup"><span data-stu-id="6ec00-107">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>
## <a name="members"></a><span data-ttu-id="6ec00-108">Membros</span><span class="sxs-lookup"><span data-stu-id="6ec00-108">Members</span></span>
|<span data-ttu-id="6ec00-109">Membro</span><span class="sxs-lookup"><span data-stu-id="6ec00-109">Member</span></span>|<span data-ttu-id="6ec00-110">Valor</span><span class="sxs-lookup"><span data-stu-id="6ec00-110">Value</span></span>|<span data-ttu-id="6ec00-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ec00-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ec00-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="6ec00-112">userDefined</span></span>|<span data-ttu-id="6ec00-113">0</span><span class="sxs-lookup"><span data-stu-id="6ec00-113">0</span></span>|<span data-ttu-id="6ec00-114">Permitir que o usuário pode definir.</span><span class="sxs-lookup"><span data-stu-id="6ec00-114">Allow the user to set.</span></span>|
|<span data-ttu-id="6ec00-115">nenhum</span><span class="sxs-lookup"><span data-stu-id="6ec00-115">none</span></span>|<span data-ttu-id="6ec00-116">1</span><span class="sxs-lookup"><span data-stu-id="6ec00-116">1</span></span>|<span data-ttu-id="6ec00-117">Nenhum dado de telemetria é enviado de componentes do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="6ec00-117">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="6ec00-118">Observação: Esse valor só é aplicável aos dispositivos enterprise e servidor.</span><span class="sxs-lookup"><span data-stu-id="6ec00-118">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="6ec00-119">O uso dessa configuração em outros dispositivos é equivalente a definir o valor de 1.</span><span class="sxs-lookup"><span data-stu-id="6ec00-119">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="6ec00-120">básico</span><span class="sxs-lookup"><span data-stu-id="6ec00-120">basic</span></span>|<span data-ttu-id="6ec00-121">2</span><span class="sxs-lookup"><span data-stu-id="6ec00-121">2</span></span>|<span data-ttu-id="6ec00-122">Envia dados de Telemetria básica.</span><span class="sxs-lookup"><span data-stu-id="6ec00-122">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="6ec00-123">Avançado</span><span class="sxs-lookup"><span data-stu-id="6ec00-123">enhanced</span></span>|<span data-ttu-id="6ec00-124">3</span><span class="sxs-lookup"><span data-stu-id="6ec00-124">3</span></span>|<span data-ttu-id="6ec00-125">Envia aprimorado de dados de telemetria, incluindo dados de uso e ideias.</span><span class="sxs-lookup"><span data-stu-id="6ec00-125">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="6ec00-126">completo</span><span class="sxs-lookup"><span data-stu-id="6ec00-126">full</span></span>|<span data-ttu-id="6ec00-127">4</span><span class="sxs-lookup"><span data-stu-id="6ec00-127">4</span></span>|<span data-ttu-id="6ec00-128">Envia dados de telemetria completo incluindo dados de diagnósticos, como o estado do sistema.</span><span class="sxs-lookup"><span data-stu-id="6ec00-128">Sends full telemetry data including diagnostic data, such as system state.</span></span>|





