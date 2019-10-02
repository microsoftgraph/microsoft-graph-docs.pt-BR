---
title: Registrar dispositivos para o gerenciamento no Intune
description: " O registro (BYOD) permite que os usuários registrem seus telefones, tablets ou computadores pessoais. O registro de dispositivo de propriedade corporativa (COD) permite cenários de gerenciamento como apagamento remoto, dispositivos compartilhados ou afinidade de usuários em um dispositivo."
localization_priority: Normal
author: davidmu1
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 54a2a8bb3901f1a6938401963e8efcbd9e02f194
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360584"
---
# <a name="enroll-devices-for-management-in-intune"></a><span data-ttu-id="a23cd-104">Registrar dispositivos para o gerenciamento no Intune</span><span class="sxs-lookup"><span data-stu-id="a23cd-104">Enroll devices for management in Intune</span></span>

> <span data-ttu-id="a23cd-105">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a23cd-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="a23cd-106">É possível registrar dispositivos, incluindo computadores Windows, para habilitar o gerenciamento de dispositivo móvel (MDM) com o Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="a23cd-106">You can enroll devices, including Windows PCs, to enable mobile device management (MDM) with Microsoft Intune.</span></span> <span data-ttu-id="a23cd-107">Este tópico descreve as diferentes maneiras de registrar dispositivos móveis no gerenciamento do Intune.</span><span class="sxs-lookup"><span data-stu-id="a23cd-107">This topic describes different ways to enroll mobile devices in Intune management.</span></span> <span data-ttu-id="a23cd-108">A maneira de registrar dispositivos depende do tipo de dispositivo, da propriedade e do nível de gerenciamento necessário.</span><span class="sxs-lookup"><span data-stu-id="a23cd-108">The way you enroll your devices depends on the device type, ownership, and the level of management that's needed.</span></span> <span data-ttu-id="a23cd-109">O registro "Traga seu próprio dispositivo" (BYOD) permite aos usuários registrar seus telefones, computador e tablets pessoais.</span><span class="sxs-lookup"><span data-stu-id="a23cd-109">"Bring your own device" (BYOD) enrollment lets users enroll their personal phones, tablets, or PCs.</span></span> <span data-ttu-id="a23cd-110">O registro de dispositivo de propriedade corporativa (COD) permite cenários de gerenciamento como apagamento remoto, dispositivos compartilhados ou afinidade de usuários em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a23cd-110">Corporate-owned device (COD) enrollment enables management scenarios like remote wipe, shared devices, or user affinity for a device.</span></span>

<span data-ttu-id="a23cd-111">Os seguintes recursos do Graph estão disponíveis para gerenciar registros no Intune:</span><span class="sxs-lookup"><span data-stu-id="a23cd-111">The following Graph resources are available to manage enrollment in Intune:</span></span>  

- [<span data-ttu-id="a23cd-112">Configuração de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a23cd-112">Device enrollment configuration</span></span>](intune-onboarding-deviceenrollmentconfiguration.md)
- [<span data-ttu-id="a23cd-113">Configuração de limite do registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a23cd-113">Device enrollment limit configuration</span></span>](intune-onboarding-deviceenrollmentlimitconfiguration.md)
- [<span data-ttu-id="a23cd-114">Restrição da plataforma de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a23cd-114">Device enrollment platform restriction</span></span>](intune-onboarding-deviceenrollmentplatformrestriction.md)
- [<span data-ttu-id="a23cd-115">Configuração das restrições da plataforma de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a23cd-115">Device enrollment platform restrictions configuration</span></span>](intune-onboarding-deviceenrollmentplatformrestrictionsconfiguration.md)
- [<span data-ttu-id="a23cd-116">Configuração do Windows Hello para empresas do registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a23cd-116">Device enrollment Windows Hello for business configuration</span></span>](intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)
- [<span data-ttu-id="a23cd-117">Conector do Exchange de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="a23cd-117">Device management exchange connector</span></span>](intune-onboarding-devicemanagementexchangeconnector.md)
- [<span data-ttu-id="a23cd-118">Status do conector do Exchange de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="a23cd-118">Device management exchange connector status</span></span>](intune-onboarding-devicemanagementexchangeconnectorstatus.md)
- [<span data-ttu-id="a23cd-119">Tipo de sincronização do conector do Exchange de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="a23cd-119">Device management exchange connector sync type</span></span>](intune-onboarding-devicemanagementexchangeconnectorsynctype.md)
- [<span data-ttu-id="a23cd-120">Tipo de conector do Exchange de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="a23cd-120">Device management exchange connector type</span></span>](intune-onboarding-devicemanagementexchangeconnectortype.md)
- [<span data-ttu-id="a23cd-121">Parceiro de gerenciamento do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a23cd-121">Device management partner</span></span>](intune-onboarding-devicemanagementpartner.md)
- [<span data-ttu-id="a23cd-122">Tipo de aplicativo de parceiro de gerenciamento do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a23cd-122">Device management partner app type</span></span>](intune-onboarding-devicemanagementpartnerapptype.md)
- [<span data-ttu-id="a23cd-123">Estado de locatário de parceiro de gerenciamento do dispositivo</span><span class="sxs-lookup"><span data-stu-id="a23cd-123">Device management partner tenant state</span></span>](intune-onboarding-devicemanagementpartnertenantstate.md)
- [<span data-ttu-id="a23cd-124">Habilitação</span><span class="sxs-lookup"><span data-stu-id="a23cd-124">Enablement</span></span>](intune-onboarding-enablement.md)
- [<span data-ttu-id="a23cd-125">Atribuição de configuração do registro</span><span class="sxs-lookup"><span data-stu-id="a23cd-125">Enrollment configuration assignment</span></span>](intune-onboarding-enrollmentconfigurationassignment.md)
- [<span data-ttu-id="a23cd-126">Marca Intune</span><span class="sxs-lookup"><span data-stu-id="a23cd-126">Intune brand</span></span>](intune-onboarding-intunebrand.md)
- [<span data-ttu-id="a23cd-127">Autoridade MDM</span><span class="sxs-lookup"><span data-stu-id="a23cd-127">MDM authority</span></span>](intune-onboarding-mdmauthority.md)
- [<span data-ttu-id="a23cd-128">Conector de defesa contra ameaças móveis</span><span class="sxs-lookup"><span data-stu-id="a23cd-128">Mobile threat defense connector</span></span>](intune-onboarding-mobilethreatdefenseconnector.md)
- [<span data-ttu-id="a23cd-129">Estado de locatário do parceiro de ameaças móveis</span><span class="sxs-lookup"><span data-stu-id="a23cd-129">Mobile threat partner tenant state</span></span>](intune-onboarding-mobilethreatpartnertenantstate.md)
- [<span data-ttu-id="a23cd-130">Configuração de acesso condicional local</span><span class="sxs-lookup"><span data-stu-id="a23cd-130">On-premises conditional access settings</span></span>](intune-onboarding-onpremisesconditionalaccesssettings.md)
- [<span data-ttu-id="a23cd-131">Organização</span><span class="sxs-lookup"><span data-stu-id="a23cd-131">Organization</span></span>](intune-onboarding-organization.md)
- [<span data-ttu-id="a23cd-132">Cores RGB</span><span class="sxs-lookup"><span data-stu-id="a23cd-132">RGB color</span></span>](intune-onboarding-rgbcolor.md)
- [<span data-ttu-id="a23cd-133">Token VPP</span><span class="sxs-lookup"><span data-stu-id="a23cd-133">VPP token</span></span>](intune-onboarding-vpptoken.md)
- [<span data-ttu-id="a23cd-134">Estado do token VPP</span><span class="sxs-lookup"><span data-stu-id="a23cd-134">VPP token state</span></span>](intune-onboarding-vpptokenstate.md)
- [<span data-ttu-id="a23cd-135">Status de sincronização do token VPP</span><span class="sxs-lookup"><span data-stu-id="a23cd-135">VPP token sync status</span></span>](intune-onboarding-vpptokensyncstatus.md)
- [<span data-ttu-id="a23cd-136">Uso do PIN do Windows Hello para empresas</span><span class="sxs-lookup"><span data-stu-id="a23cd-136">Windows Hello for business PIN usage</span></span>](intune-onboarding-windowshelloforbusinesspinusage.md)

