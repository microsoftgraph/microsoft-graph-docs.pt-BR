---
title: tipo de enum habilitação
description: 'Valores usados para indicar o status de um dispositivo. '
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 539d57111003f348147a6be3952d969ab4206b5d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911956"
---
# <a name="enablement-enum-type"></a><span data-ttu-id="c47f1-103">tipo de enum habilitação</span><span class="sxs-lookup"><span data-stu-id="c47f1-103">enablement enum type</span></span>

> <span data-ttu-id="c47f1-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c47f1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c47f1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c47f1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c47f1-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c47f1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c47f1-107">Valores usados para indicar o status de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c47f1-107">Values used to indicate the status of a device.</span></span> 

<span data-ttu-id="c47f1-108">Observe que há uma diferença entre desabilitado e não configurado.</span><span class="sxs-lookup"><span data-stu-id="c47f1-108">Note that there is a difference between disabled and not configured.</span></span>

## <a name="members"></a><span data-ttu-id="c47f1-109">Membros</span><span class="sxs-lookup"><span data-stu-id="c47f1-109">Members</span></span>
|<span data-ttu-id="c47f1-110">Membro</span><span class="sxs-lookup"><span data-stu-id="c47f1-110">Member</span></span>|<span data-ttu-id="c47f1-111">Valor</span><span class="sxs-lookup"><span data-stu-id="c47f1-111">Value</span></span>|<span data-ttu-id="c47f1-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="c47f1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c47f1-113">não-configuradas</span><span class="sxs-lookup"><span data-stu-id="c47f1-113">notConfigured</span></span>|<span data-ttu-id="c47f1-114">0</span><span class="sxs-lookup"><span data-stu-id="c47f1-114">0</span></span>|<span data-ttu-id="c47f1-115">Valor de padrão de dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="c47f1-115">Device default value, no intent.</span></span>|
|<span data-ttu-id="c47f1-116">enabled</span><span class="sxs-lookup"><span data-stu-id="c47f1-116">enabled</span></span>|<span data-ttu-id="c47f1-117">1</span><span class="sxs-lookup"><span data-stu-id="c47f1-117">1</span></span>|<span data-ttu-id="c47f1-118">Permite a configuração no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c47f1-118">Enables the setting on the device.</span></span>|
|<span data-ttu-id="c47f1-119">desabilitado</span><span class="sxs-lookup"><span data-stu-id="c47f1-119">disabled</span></span>|<span data-ttu-id="c47f1-120">2</span><span class="sxs-lookup"><span data-stu-id="c47f1-120">2</span></span>|<span data-ttu-id="c47f1-121">Desativa a configuração no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c47f1-121">Disables the setting on the device.</span></span>|
