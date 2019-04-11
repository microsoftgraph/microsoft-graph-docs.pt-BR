---
title: tipo de enumeração configurationManagerClientState
description: Estado do cliente de gerenciador de configurações
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1f6231ecebf407172f2c7178a130d90200868292
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31776518"
---
# <a name="configurationmanagerclientstate-enum-type"></a><span data-ttu-id="2bdba-103">tipo de enumeração configurationManagerClientState</span><span class="sxs-lookup"><span data-stu-id="2bdba-103">configurationManagerClientState enum type</span></span>

> <span data-ttu-id="2bdba-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2bdba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2bdba-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2bdba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2bdba-106">Estado do cliente de gerenciador de configurações</span><span class="sxs-lookup"><span data-stu-id="2bdba-106">Configuration manager client state</span></span>

## <a name="members"></a><span data-ttu-id="2bdba-107">Membros</span><span class="sxs-lookup"><span data-stu-id="2bdba-107">Members</span></span>
|<span data-ttu-id="2bdba-108">Membro</span><span class="sxs-lookup"><span data-stu-id="2bdba-108">Member</span></span>|<span data-ttu-id="2bdba-109">Valor</span><span class="sxs-lookup"><span data-stu-id="2bdba-109">Value</span></span>|<span data-ttu-id="2bdba-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2bdba-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2bdba-111">desconhecido</span><span class="sxs-lookup"><span data-stu-id="2bdba-111">unknown</span></span>|<span data-ttu-id="2bdba-112">,0</span><span class="sxs-lookup"><span data-stu-id="2bdba-112">0</span></span>|<span data-ttu-id="2bdba-113">O agente do Gerenciador de configurações é mais antigo que 1806 ou não instalado ou este dispositivo não foi verificado no Intune por mais de 30 dias.</span><span class="sxs-lookup"><span data-stu-id="2bdba-113">Configuration manager agent is older than 1806 or not installed or this device has not checked into Intune for over 30 days.</span></span>|
|<span data-ttu-id="2bdba-114">instalação</span><span class="sxs-lookup"><span data-stu-id="2bdba-114">installed</span></span>|<span data-ttu-id="2bdba-115">1</span><span class="sxs-lookup"><span data-stu-id="2bdba-115">1</span></span>|<span data-ttu-id="2bdba-116">O agente do Gerenciador de configurações está instalado, mas talvez ainda não esteja aparecendo no console do Gerenciador de configurações.</span><span class="sxs-lookup"><span data-stu-id="2bdba-116">The configuration manager agent is installed but may not be showing up in the configuration manager console yet.</span></span> <span data-ttu-id="2bdba-117">Aguarde algumas horas para que ele seja atualizado.</span><span class="sxs-lookup"><span data-stu-id="2bdba-117">Wait a few hours for it to refresh.</span></span>|
|<span data-ttu-id="2bdba-118">condições</span><span class="sxs-lookup"><span data-stu-id="2bdba-118">healthy</span></span>|<span data-ttu-id="2bdba-119">178</span><span class="sxs-lookup"><span data-stu-id="2bdba-119">7</span></span>|<span data-ttu-id="2bdba-120">Este dispositivo pôde fazer check-in com o serviço do Gerenciador de configurações com êxito.</span><span class="sxs-lookup"><span data-stu-id="2bdba-120">This device was able to check in with the configuration manager service successfully.</span></span>|
|<span data-ttu-id="2bdba-121">installFailed</span><span class="sxs-lookup"><span data-stu-id="2bdba-121">installFailed</span></span>|<span data-ttu-id="2bdba-122">8</span><span class="sxs-lookup"><span data-stu-id="2bdba-122">8</span></span>|<span data-ttu-id="2bdba-123">Falha ao instalar o agente do Gerenciador de configurações.</span><span class="sxs-lookup"><span data-stu-id="2bdba-123">The configuration manager agent failed to install.</span></span>|
|<span data-ttu-id="2bdba-124">updateFailed</span><span class="sxs-lookup"><span data-stu-id="2bdba-124">updateFailed</span></span>|<span data-ttu-id="2bdba-125">11</span><span class="sxs-lookup"><span data-stu-id="2bdba-125">11</span></span>|<span data-ttu-id="2bdba-126">A atualização da versão x para a versão y do agente do Gerenciador de configuração falhou.</span><span class="sxs-lookup"><span data-stu-id="2bdba-126">The update from version x to version y of the configuration manager agent failed.</span></span> |
|<span data-ttu-id="2bdba-127">communicationError</span><span class="sxs-lookup"><span data-stu-id="2bdba-127">communicationError</span></span>|<span data-ttu-id="2bdba-128">19</span><span class="sxs-lookup"><span data-stu-id="2bdba-128">19</span></span>|<span data-ttu-id="2bdba-129">O agente do Gerenciador de configurações pôde acessar o serviço do Configuration Manager no passado, mas agora não é mais possível.</span><span class="sxs-lookup"><span data-stu-id="2bdba-129">The configuration manager agent was able to reach the configuration manager service in the past but is now no longer able to.</span></span> |





