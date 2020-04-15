---
title: Gerenciamento de despesas com telecomunicações no Microsoft Intune
description: É possível limitar o uso e o roaming de dados em dispositivos de propriedade corporativa ao usar o serviço de gerenciamento de despesas com telecomunicações Saaswedo, que é integrado ao Intune. O serviço permite configurar e impor limites de uso e enviar aos usuários um alerta quando eles excederem um limite configurado. Também é possível configurar o serviço para realizar outras ações, como a desabilitação do roaming, quando os usuários excederem o limite. Relatórios com informações sobre o uso e o monitoramento dos dados estão disponíveis no console do Saaswedo. Antes de usar o serviço de gerenciamento de despesas com telecomunicações Saaswedo com o Intune, é preciso definir as configurações em um console do Saaswedo e no Intune. A conexão deve ser ativada para o serviço Saaswedo e para o Intune. Se a conexão do lado do Saaswedo estiver habilitada, mas a do lado do Intune não estiver, o Intune receberá a comunicação, mas ela será ignorada.
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: c93338c39a2dfce144688fb7c042d6e520ed6ac8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43445572"
---
# <a name="telecom-expense-management-in-microsoft-intune"></a><span data-ttu-id="1b3f1-109">Gerenciamento de despesas com telecomunicações no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="1b3f1-109">Telecom expense management in Microsoft Intune</span></span>

<span data-ttu-id="1b3f1-110">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b3f1-110">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1b3f1-111">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1b3f1-111">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="1b3f1-112">É possível limitar o uso e o roaming de dados em dispositivos de propriedade corporativa ao usar o serviço de gerenciamento de despesas com telecomunicações Saaswedo, que é integrado ao Intune.</span><span class="sxs-lookup"><span data-stu-id="1b3f1-112">You can limit data usage and roaming on corporate-owned devices when you use the Saaswedo telecom expense management service, which integrates with Intune.</span></span> <span data-ttu-id="1b3f1-113">O serviço permite configurar e impor limites de uso e enviar aos usuários um alerta quando eles excederem um limite configurado.</span><span class="sxs-lookup"><span data-stu-id="1b3f1-113">The service enables you to set and enforce usage limits and to send users an alert when they exceed a configured threshold.</span></span> <span data-ttu-id="1b3f1-114">Também é possível configurar o serviço para realizar outras ações, como a desabilitação do roaming, quando os usuários excederem o limite.</span><span class="sxs-lookup"><span data-stu-id="1b3f1-114">You can also configure the service to take different actions, such as disabling roaming, when users exceed the threshold.</span></span> <span data-ttu-id="1b3f1-115">Relatórios com informações sobre o uso e o monitoramento dos dados estão disponíveis no console do Saaswedo.</span><span class="sxs-lookup"><span data-stu-id="1b3f1-115">Reports that provide data usage and monitoring information are available in the Saaswedo console.</span></span> <span data-ttu-id="1b3f1-116">Antes de usar o serviço de gerenciamento de despesas com telecomunicações Saaswedo com o Intune, é preciso definir as configurações em um console do Saaswedo e no Intune.</span><span class="sxs-lookup"><span data-stu-id="1b3f1-116">Before you can use the Saaswedo telecom expense management service with Intune, you need to configure settings in a Saaswedo console and in Intune.</span></span> <span data-ttu-id="1b3f1-117">A conexão deve ser ativada para o serviço Saaswedo e para o Intune.</span><span class="sxs-lookup"><span data-stu-id="1b3f1-117">The connection must be turned on for the Saaswedo service and for Intune.</span></span> <span data-ttu-id="1b3f1-118">Se a conexão do lado do Saaswedo estiver habilitada, mas a do lado do Intune não estiver, o Intune receberá a comunicação, mas ela será ignorada.</span><span class="sxs-lookup"><span data-stu-id="1b3f1-118">If the Saaswedo side of the connection is enabled, but not the Intune side, Intune receives the communication, but ignores it.</span></span>

<span data-ttu-id="1b3f1-119">Os seguintes recursos do Graph estão disponíveis para gerenciar despesas com telecomunicações no Intune:</span><span class="sxs-lookup"><span data-stu-id="1b3f1-119">The following Graph resources are available to manage telecom expenses in Intune:</span></span>  

- [<span data-ttu-id="1b3f1-120">Parceiro de gerenciamento de despesas com telecomunicações</span><span class="sxs-lookup"><span data-stu-id="1b3f1-120">Telecom expense management partner</span></span>](intune-tem-telecomexpensemanagementpartner.md)




