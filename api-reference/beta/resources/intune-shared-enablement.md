---
title: tipo de enum habilitação
description: 'Valores usados para indicar o status de um dispositivo. '
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c77da7026640e9ad0a6f6f08f077d509cb411f22
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888253"
---
# <a name="enablement-enum-type"></a><span data-ttu-id="19171-103">tipo de enum habilitação</span><span class="sxs-lookup"><span data-stu-id="19171-103">enablement enum type</span></span>

> <span data-ttu-id="19171-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="19171-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="19171-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="19171-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="19171-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="19171-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="19171-107">Valores usados para indicar o status de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="19171-107">Values used to indicate the status of a device.</span></span> 

<span data-ttu-id="19171-108">Observe que há uma diferença entre desabilitado e não configurado.</span><span class="sxs-lookup"><span data-stu-id="19171-108">Note that there is a difference between disabled and not configured.</span></span>

## <a name="members"></a><span data-ttu-id="19171-109">Membros</span><span class="sxs-lookup"><span data-stu-id="19171-109">Members</span></span>
|<span data-ttu-id="19171-110">Membro</span><span class="sxs-lookup"><span data-stu-id="19171-110">Member</span></span>|<span data-ttu-id="19171-111">Valor</span><span class="sxs-lookup"><span data-stu-id="19171-111">Value</span></span>|<span data-ttu-id="19171-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="19171-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19171-113">não-configuradas</span><span class="sxs-lookup"><span data-stu-id="19171-113">notConfigured</span></span>|<span data-ttu-id="19171-114">0</span><span class="sxs-lookup"><span data-stu-id="19171-114">0</span></span>|<span data-ttu-id="19171-115">Valor de padrão de dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="19171-115">Device default value, no intent.</span></span>|
|<span data-ttu-id="19171-116">enabled</span><span class="sxs-lookup"><span data-stu-id="19171-116">enabled</span></span>|<span data-ttu-id="19171-117">1</span><span class="sxs-lookup"><span data-stu-id="19171-117">1</span></span>|<span data-ttu-id="19171-118">Permite a configuração no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="19171-118">Enables the setting on the device.</span></span>|
|<span data-ttu-id="19171-119">desabilitado</span><span class="sxs-lookup"><span data-stu-id="19171-119">disabled</span></span>|<span data-ttu-id="19171-120">2</span><span class="sxs-lookup"><span data-stu-id="19171-120">2</span></span>|<span data-ttu-id="19171-121">Desativa a configuração no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="19171-121">Disables the setting on the device.</span></span>|
