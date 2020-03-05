---
title: Registrar dispositivos para o gerenciamento no Intune
description: " O registro (BYOD) permite que os usuários registrem seus telefones, tablets ou computadores pessoais. O registro de dispositivo de propriedade corporativa (COD) permite cenários de gerenciamento como apagamento remoto, dispositivos compartilhados ou afinidade de usuários em um dispositivo."
localization_priority: Normal
author: davidmu1
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 171a58e82ea3e7ab76d919d1fef693f540b4f4db
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448162"
---
# <a name="enroll-devices-for-management-in-intune"></a><span data-ttu-id="424c3-104">Registrar dispositivos para o gerenciamento no Intune</span><span class="sxs-lookup"><span data-stu-id="424c3-104">Enroll devices for management in Intune</span></span>

<span data-ttu-id="424c3-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="424c3-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="424c3-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="424c3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="424c3-107">É possível registrar dispositivos, incluindo computadores Windows, para habilitar o gerenciamento de dispositivo móvel (MDM) com o Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="424c3-107">You can enroll devices, including Windows PCs, to enable mobile device management (MDM) with Microsoft Intune.</span></span> <span data-ttu-id="424c3-108">Este tópico descreve as diferentes maneiras de registrar dispositivos móveis no gerenciamento do Intune.</span><span class="sxs-lookup"><span data-stu-id="424c3-108">This topic describes different ways to enroll mobile devices in Intune management.</span></span> <span data-ttu-id="424c3-109">A maneira de registrar dispositivos depende do tipo de dispositivo, da propriedade e do nível de gerenciamento necessário.</span><span class="sxs-lookup"><span data-stu-id="424c3-109">The way you enroll your devices depends on the device type, ownership, and the level of management that's needed.</span></span> <span data-ttu-id="424c3-110">O registro "Traga seu próprio dispositivo" (BYOD) permite aos usuários registrar seus telefones, computador e tablets pessoais.</span><span class="sxs-lookup"><span data-stu-id="424c3-110">"Bring your own device" (BYOD) enrollment lets users enroll their personal phones, tablets, or PCs.</span></span> <span data-ttu-id="424c3-111">O registro de dispositivo de propriedade corporativa (COD) permite cenários de gerenciamento como apagamento remoto, dispositivos compartilhados ou afinidade de usuários em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="424c3-111">Corporate-owned device (COD) enrollment enables management scenarios like remote wipe, shared devices, or user affinity for a device.</span></span>

<span data-ttu-id="424c3-112">Os seguintes recursos do Graph estão disponíveis para gerenciar registros no Intune:</span><span class="sxs-lookup"><span data-stu-id="424c3-112">The following Graph resources are available to manage enrollment in Intune:</span></span>  

- [<span data-ttu-id="424c3-113">Configuração de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="424c3-113">Device enrollment configuration</span></span>](intune-onboarding-deviceenrollmentconfiguration.md)
- [<span data-ttu-id="424c3-114">Configuração de limite do registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="424c3-114">Device enrollment limit configuration</span></span>](intune-onboarding-deviceenrollmentlimitconfiguration.md)
- [<span data-ttu-id="424c3-115">Restrição da plataforma de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="424c3-115">Device enrollment platform restriction</span></span>](intune-onboarding-deviceenrollmentplatformrestriction.md)
- [<span data-ttu-id="424c3-116">Configuração das restrições da plataforma de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="424c3-116">Device enrollment platform restrictions configuration</span></span>](intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)
- [<span data-ttu-id="424c3-117">Configuração do Windows Hello para empresas do registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="424c3-117">Device enrollment Windows Hello for business configuration</span></span>](intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)
- [<span data-ttu-id="424c3-118">Conector do Exchange de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="424c3-118">Device management exchange connector</span></span>](intune-onboarding-devicemanagementexchangeconnector.md)
- [<span data-ttu-id="424c3-119">Status do conector do Exchange de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="424c3-119">Device management exchange connector status</span></span>](intune-onboarding-devicemanagementexchangeconnectorstatus.md)
- [<span data-ttu-id="424c3-120">Tipo de sincronização do conector do Exchange de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="424c3-120">Device management exchange connector sync type</span></span>](intune-onboarding-devicemanagementexchangeconnectorsynctype.md)
- [<span data-ttu-id="424c3-121">Tipo de conector do Exchange de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="424c3-121">Device management exchange connector type</span></span>](intune-onboarding-devicemanagementexchangeconnectortype.md)
- [<span data-ttu-id="424c3-122">Parceiro de gerenciamento do dispositivo</span><span class="sxs-lookup"><span data-stu-id="424c3-122">Device management partner</span></span>](intune-onboarding-devicemanagementpartner.md)
- [<span data-ttu-id="424c3-123">Tipo de aplicativo de parceiro de gerenciamento do dispositivo</span><span class="sxs-lookup"><span data-stu-id="424c3-123">Device management partner app type</span></span>](intune-onboarding-devicemanagementpartnerapptype.md)
- [<span data-ttu-id="424c3-124">Estado de locatário de parceiro de gerenciamento do dispositivo</span><span class="sxs-lookup"><span data-stu-id="424c3-124">Device management partner tenant state</span></span>](intune-onboarding-devicemanagementpartnertenantstate.md)
- [<span data-ttu-id="424c3-125">Habilitação</span><span class="sxs-lookup"><span data-stu-id="424c3-125">Enablement</span></span>](intune-onboarding-enablement.md)
- [<span data-ttu-id="424c3-126">Atribuição de configuração do registro</span><span class="sxs-lookup"><span data-stu-id="424c3-126">Enrollment configuration assignment</span></span>](intune-onboarding-enrollmentconfigurationassignment.md)
- [<span data-ttu-id="424c3-127">Marca Intune</span><span class="sxs-lookup"><span data-stu-id="424c3-127">Intune brand</span></span>](intune-onboarding-intunebrand.md)
- [<span data-ttu-id="424c3-128">Autoridade MDM</span><span class="sxs-lookup"><span data-stu-id="424c3-128">MDM authority</span></span>](intune-onboarding-mdmauthority.md)
- [<span data-ttu-id="424c3-129">Conector de defesa contra ameaças móveis</span><span class="sxs-lookup"><span data-stu-id="424c3-129">Mobile threat defense connector</span></span>](intune-onboarding-mobilethreatdefenseconnector.md)
- [<span data-ttu-id="424c3-130">Estado de locatário do parceiro de ameaças móveis</span><span class="sxs-lookup"><span data-stu-id="424c3-130">Mobile threat partner tenant state</span></span>](intune-onboarding-mobilethreatpartnertenantstate.md)
- [<span data-ttu-id="424c3-131">Configuração de acesso condicional local</span><span class="sxs-lookup"><span data-stu-id="424c3-131">On-premises conditional access settings</span></span>](intune-onboarding-onpremisesconditionalaccesssettings.md)
- [<span data-ttu-id="424c3-132">Organização</span><span class="sxs-lookup"><span data-stu-id="424c3-132">Organization</span></span>](intune-onboarding-organization.md)
- [<span data-ttu-id="424c3-133">Cores RGB</span><span class="sxs-lookup"><span data-stu-id="424c3-133">RGB color</span></span>](intune-onboarding-rgbcolor.md)
- [<span data-ttu-id="424c3-134">Token VPP</span><span class="sxs-lookup"><span data-stu-id="424c3-134">VPP token</span></span>](intune-onboarding-vpptoken.md)
- [<span data-ttu-id="424c3-135">Estado do token VPP</span><span class="sxs-lookup"><span data-stu-id="424c3-135">VPP token state</span></span>](intune-onboarding-vpptokenstate.md)
- [<span data-ttu-id="424c3-136">Status de sincronização do token VPP</span><span class="sxs-lookup"><span data-stu-id="424c3-136">VPP token sync status</span></span>](intune-onboarding-vpptokensyncstatus.md)
- [<span data-ttu-id="424c3-137">Uso do PIN do Windows Hello para empresas</span><span class="sxs-lookup"><span data-stu-id="424c3-137">Windows Hello for business PIN usage</span></span>](intune-onboarding-windowshelloforbusinesspinusage.md)

