---
title: tipo de enum habilitação
description: 'Valores usados para indicar o status de um dispositivo. '
ms.openlocfilehash: 5e72df98d33a7d3502dae4bc369781b69bc6aeb0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036767"
---
# <a name="enablement-enum-type"></a><span data-ttu-id="4e16f-103">tipo de enum habilitação</span><span class="sxs-lookup"><span data-stu-id="4e16f-103">enablement enum type</span></span>

> <span data-ttu-id="4e16f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4e16f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4e16f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4e16f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4e16f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4e16f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4e16f-107">Valores usados para indicar o status de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4e16f-107">Values used to indicate the status of a device.</span></span> 

<span data-ttu-id="4e16f-108">Observe que há uma diferença entre desabilitado e não configurado.</span><span class="sxs-lookup"><span data-stu-id="4e16f-108">Note that there is a difference between disabled and not configured.</span></span>

## <a name="members"></a><span data-ttu-id="4e16f-109">Membros</span><span class="sxs-lookup"><span data-stu-id="4e16f-109">Members</span></span>
|<span data-ttu-id="4e16f-110">Membro</span><span class="sxs-lookup"><span data-stu-id="4e16f-110">Member</span></span>|<span data-ttu-id="4e16f-111">Valor</span><span class="sxs-lookup"><span data-stu-id="4e16f-111">Value</span></span>|<span data-ttu-id="4e16f-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e16f-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e16f-113">não-configuradas</span><span class="sxs-lookup"><span data-stu-id="4e16f-113">notConfigured</span></span>|<span data-ttu-id="4e16f-114">0</span><span class="sxs-lookup"><span data-stu-id="4e16f-114">0</span></span>|<span data-ttu-id="4e16f-115">Valor de padrão de dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="4e16f-115">Device default value, no intent.</span></span>|
|<span data-ttu-id="4e16f-116">enabled</span><span class="sxs-lookup"><span data-stu-id="4e16f-116">enabled</span></span>|<span data-ttu-id="4e16f-117">1</span><span class="sxs-lookup"><span data-stu-id="4e16f-117">1</span></span>|<span data-ttu-id="4e16f-118">Permite a configuração no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4e16f-118">Enables the setting on the device.</span></span>|
|<span data-ttu-id="4e16f-119">desabilitado</span><span class="sxs-lookup"><span data-stu-id="4e16f-119">disabled</span></span>|<span data-ttu-id="4e16f-120">2</span><span class="sxs-lookup"><span data-stu-id="4e16f-120">2</span></span>|<span data-ttu-id="4e16f-121">Desativa a configuração no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4e16f-121">Disables the setting on the device.</span></span>|
