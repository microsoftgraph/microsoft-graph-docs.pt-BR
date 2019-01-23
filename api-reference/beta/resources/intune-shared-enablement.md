---
title: tipo de enum habilitação
description: Descreve a enumeração de habilitação da API Microsoft Graph para Intune, que oferece suporte a vários fluxos de trabalho.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 538b52790cf7748453adfda2a6bea8334a36fb87
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399560"
---
# <a name="enablement-enum-type"></a><span data-ttu-id="d5e7d-103">tipo de enum habilitação</span><span class="sxs-lookup"><span data-stu-id="d5e7d-103">enablement enum type</span></span>

> <span data-ttu-id="d5e7d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d5e7d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d5e7d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d5e7d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d5e7d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d5e7d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d5e7d-107">Valores usados para indicar o status de um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d5e7d-107">Values used to indicate the status of a device.</span></span> 

<span data-ttu-id="d5e7d-108">Observe que há uma diferença entre desabilitado e não configurado.</span><span class="sxs-lookup"><span data-stu-id="d5e7d-108">Note that there is a difference between disabled and not configured.</span></span>

## <a name="members"></a><span data-ttu-id="d5e7d-109">Membros</span><span class="sxs-lookup"><span data-stu-id="d5e7d-109">Members</span></span>
|<span data-ttu-id="d5e7d-110">Membro</span><span class="sxs-lookup"><span data-stu-id="d5e7d-110">Member</span></span>|<span data-ttu-id="d5e7d-111">Valor</span><span class="sxs-lookup"><span data-stu-id="d5e7d-111">Value</span></span>|<span data-ttu-id="d5e7d-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5e7d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5e7d-113">não-configuradas</span><span class="sxs-lookup"><span data-stu-id="d5e7d-113">notConfigured</span></span>|<span data-ttu-id="d5e7d-114">0</span><span class="sxs-lookup"><span data-stu-id="d5e7d-114">0</span></span>|<span data-ttu-id="d5e7d-115">Valor de padrão de dispositivo, sem intenção.</span><span class="sxs-lookup"><span data-stu-id="d5e7d-115">Device default value, no intent.</span></span>|
|<span data-ttu-id="d5e7d-116">enabled</span><span class="sxs-lookup"><span data-stu-id="d5e7d-116">enabled</span></span>|<span data-ttu-id="d5e7d-117">1</span><span class="sxs-lookup"><span data-stu-id="d5e7d-117">1</span></span>|<span data-ttu-id="d5e7d-118">Permite a configuração no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d5e7d-118">Enables the setting on the device.</span></span>|
|<span data-ttu-id="d5e7d-119">desabilitado</span><span class="sxs-lookup"><span data-stu-id="d5e7d-119">disabled</span></span>|<span data-ttu-id="d5e7d-120">2</span><span class="sxs-lookup"><span data-stu-id="d5e7d-120">2</span></span>|<span data-ttu-id="d5e7d-121">Desativa a configuração no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d5e7d-121">Disables the setting on the device.</span></span>|
