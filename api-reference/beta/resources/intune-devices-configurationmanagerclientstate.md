---
title: tipo de enum configurationManagerClientState
description: Estado de cliente do Gerenciador de configuração
author: tfitzmac
ms.openlocfilehash: dc67a5fb1c517e65da937996ed65adaa621fa3c5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354044"
---
# <a name="configurationmanagerclientstate-enum-type"></a><span data-ttu-id="5dbdf-103">tipo de enum configurationManagerClientState</span><span class="sxs-lookup"><span data-stu-id="5dbdf-103">configurationManagerClientState enum type</span></span>

> <span data-ttu-id="5dbdf-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5dbdf-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5dbdf-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5dbdf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5dbdf-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5dbdf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5dbdf-107">Estado de cliente do Gerenciador de configuração</span><span class="sxs-lookup"><span data-stu-id="5dbdf-107">Configuration manager client state</span></span>
## <a name="members"></a><span data-ttu-id="5dbdf-108">Membros</span><span class="sxs-lookup"><span data-stu-id="5dbdf-108">Members</span></span>
|<span data-ttu-id="5dbdf-109">Membro</span><span class="sxs-lookup"><span data-stu-id="5dbdf-109">Member</span></span>|<span data-ttu-id="5dbdf-110">Valor</span><span class="sxs-lookup"><span data-stu-id="5dbdf-110">Value</span></span>|<span data-ttu-id="5dbdf-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5dbdf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5dbdf-112">unknown</span><span class="sxs-lookup"><span data-stu-id="5dbdf-112">unknown</span></span>|<span data-ttu-id="5dbdf-113">0</span><span class="sxs-lookup"><span data-stu-id="5dbdf-113">0</span></span>|<span data-ttu-id="5dbdf-114">Agente do Gerenciador de configuração é mais antigo que 1806 ou não está instalado ou este dispositivo não tiver verificado em Intune por mais de 30 dias.</span><span class="sxs-lookup"><span data-stu-id="5dbdf-114">Configuration manager agent is older than 1806 or not installed or this device has not checked into Intune for over 30 days.</span></span>|
|<span data-ttu-id="5dbdf-115">instalado</span><span class="sxs-lookup"><span data-stu-id="5dbdf-115">installed</span></span>|<span data-ttu-id="5dbdf-116">1</span><span class="sxs-lookup"><span data-stu-id="5dbdf-116">1</span></span>|<span data-ttu-id="5dbdf-117">O agente do Gerenciador de configuração está instalado, mas pode não ser aparecendo no console do configuration manager ainda.</span><span class="sxs-lookup"><span data-stu-id="5dbdf-117">The configuration manager agent is installed but may not be showing up in the configuration manager console yet.</span></span> <span data-ttu-id="5dbdf-118">Aguarde algumas horas para que ele seja atualizada.</span><span class="sxs-lookup"><span data-stu-id="5dbdf-118">Wait a few hours for it to refresh.</span></span>|
|<span data-ttu-id="5dbdf-119">Íntegro</span><span class="sxs-lookup"><span data-stu-id="5dbdf-119">healthy</span></span>|<span data-ttu-id="5dbdf-120">7</span><span class="sxs-lookup"><span data-stu-id="5dbdf-120">7</span></span>|<span data-ttu-id="5dbdf-121">Este dispositivo foi capaz de check-in com o serviço do Gerenciador de configuração com êxito.</span><span class="sxs-lookup"><span data-stu-id="5dbdf-121">This device was able to check in with the configuration manager service successfully.</span></span>|
|<span data-ttu-id="5dbdf-122">installFailed</span><span class="sxs-lookup"><span data-stu-id="5dbdf-122">installFailed</span></span>|<span data-ttu-id="5dbdf-123">8</span><span class="sxs-lookup"><span data-stu-id="5dbdf-123">8</span></span>|<span data-ttu-id="5dbdf-124">Falha na instalação do agente do Gerenciador de configuração.</span><span class="sxs-lookup"><span data-stu-id="5dbdf-124">The configuration manager agent failed to install.</span></span>|
|<span data-ttu-id="5dbdf-125">updateFailed</span><span class="sxs-lookup"><span data-stu-id="5dbdf-125">updateFailed</span></span>|<span data-ttu-id="5dbdf-126">11</span><span class="sxs-lookup"><span data-stu-id="5dbdf-126">11</span></span>|<span data-ttu-id="5dbdf-127">Falha na atualização da versão x a y da versão do agente do Gerenciador de configuração.</span><span class="sxs-lookup"><span data-stu-id="5dbdf-127">The update from version x to version y of the configuration manager agent failed.</span></span> |
|<span data-ttu-id="5dbdf-128">communicationError</span><span class="sxs-lookup"><span data-stu-id="5dbdf-128">communicationError</span></span>|<span data-ttu-id="5dbdf-129">19</span><span class="sxs-lookup"><span data-stu-id="5dbdf-129">19</span></span>|<span data-ttu-id="5dbdf-130">O agente do Gerenciador de configuração foi capaz de acessar o serviço do Gerenciador de configuração no passado, mas agora não é mais possível.</span><span class="sxs-lookup"><span data-stu-id="5dbdf-130">The configuration manager agent was able to reach the configuration manager service in the past but is now no longer able to.</span></span> |





