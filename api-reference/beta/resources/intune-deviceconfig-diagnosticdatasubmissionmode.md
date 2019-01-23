---
title: tipo de enum diagnosticDataSubmissionMode
description: Permitir que o dispositivo enviar dados de telemetria de diagnóstico e uso, como Watson.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8b587d6872bcd3610c3b878ae7a672c3e776ea01
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422254"
---
# <a name="diagnosticdatasubmissionmode-enum-type"></a><span data-ttu-id="f34c7-103">tipo de enum diagnosticDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="f34c7-103">diagnosticDataSubmissionMode enum type</span></span>

> <span data-ttu-id="f34c7-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="f34c7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f34c7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f34c7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f34c7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="f34c7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f34c7-107">Permitir que o dispositivo enviar dados de telemetria de diagnóstico e uso, como Watson.</span><span class="sxs-lookup"><span data-stu-id="f34c7-107">Allow the device to send diagnostic and usage telemetry data, such as Watson.</span></span>

## <a name="members"></a><span data-ttu-id="f34c7-108">Membros</span><span class="sxs-lookup"><span data-stu-id="f34c7-108">Members</span></span>
|<span data-ttu-id="f34c7-109">Membro</span><span class="sxs-lookup"><span data-stu-id="f34c7-109">Member</span></span>|<span data-ttu-id="f34c7-110">Valor</span><span class="sxs-lookup"><span data-stu-id="f34c7-110">Value</span></span>|<span data-ttu-id="f34c7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f34c7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f34c7-112">userDefined</span><span class="sxs-lookup"><span data-stu-id="f34c7-112">userDefined</span></span>|<span data-ttu-id="f34c7-113">0</span><span class="sxs-lookup"><span data-stu-id="f34c7-113">0</span></span>|<span data-ttu-id="f34c7-114">Permitir que o usuário pode definir.</span><span class="sxs-lookup"><span data-stu-id="f34c7-114">Allow the user to set.</span></span>|
|<span data-ttu-id="f34c7-115">none</span><span class="sxs-lookup"><span data-stu-id="f34c7-115">none</span></span>|<span data-ttu-id="f34c7-116">1</span><span class="sxs-lookup"><span data-stu-id="f34c7-116">1</span></span>|<span data-ttu-id="f34c7-117">Nenhum dado de telemetria é enviado de componentes do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="f34c7-117">No telemetry data is sent from OS components.</span></span> <span data-ttu-id="f34c7-118">Observação: Esse valor só é aplicável aos dispositivos enterprise e servidor.</span><span class="sxs-lookup"><span data-stu-id="f34c7-118">Note: This value is only applicable to enterprise and server devices.</span></span> <span data-ttu-id="f34c7-119">O uso dessa configuração em outros dispositivos é equivalente a definir o valor de 1.</span><span class="sxs-lookup"><span data-stu-id="f34c7-119">Using this setting on other devices is equivalent to setting the value of 1.</span></span>|
|<span data-ttu-id="f34c7-120">básico</span><span class="sxs-lookup"><span data-stu-id="f34c7-120">basic</span></span>|<span data-ttu-id="f34c7-121">2</span><span class="sxs-lookup"><span data-stu-id="f34c7-121">2</span></span>|<span data-ttu-id="f34c7-122">Envia dados de Telemetria básica.</span><span class="sxs-lookup"><span data-stu-id="f34c7-122">Sends basic telemetry data.</span></span>|
|<span data-ttu-id="f34c7-123">Avançado</span><span class="sxs-lookup"><span data-stu-id="f34c7-123">enhanced</span></span>|<span data-ttu-id="f34c7-124">3</span><span class="sxs-lookup"><span data-stu-id="f34c7-124">3</span></span>|<span data-ttu-id="f34c7-125">Envia aprimorado de dados de telemetria, incluindo dados de uso e ideias.</span><span class="sxs-lookup"><span data-stu-id="f34c7-125">Sends enhanced telemetry data including usage and insights data.</span></span>|
|<span data-ttu-id="f34c7-126">completo</span><span class="sxs-lookup"><span data-stu-id="f34c7-126">full</span></span>|<span data-ttu-id="f34c7-127">4</span><span class="sxs-lookup"><span data-stu-id="f34c7-127">4</span></span>|<span data-ttu-id="f34c7-128">Envia dados de telemetria completo incluindo dados de diagnósticos, como o estado do sistema.</span><span class="sxs-lookup"><span data-stu-id="f34c7-128">Sends full telemetry data including diagnostic data, such as system state.</span></span>|




