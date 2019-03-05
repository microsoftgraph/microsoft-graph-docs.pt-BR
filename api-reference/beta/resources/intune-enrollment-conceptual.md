---
title: Registrar dispositivos corporativos usando o Intune-Microsoft Graph API
description: Lista a API do Microsoft Graph para os pontos de extremidade do Intune (REST) que registram dispositivos para uma organização de locatário.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 240bdc2d65d1ed8920fe1f9c067f1ffcd31a9f11
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30149830"
---
# <a name="enroll-corporate-owned-devices-by-using-intune"></a><span data-ttu-id="37886-103">Registrar dispositivos de propriedade corporativa por meio do Intune</span><span class="sxs-lookup"><span data-stu-id="37886-103">Enroll corporate-owned devices by using Intune</span></span>

> <span data-ttu-id="37886-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="37886-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="37886-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="37886-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="37886-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="37886-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="37886-107">É possível registrar dispositivos pertencentes à organização ou de propriedade corporativa para serem gerenciados com o Intune de várias maneiras, dependendo do tipo de dispositivo, de como o dispositivo foi comprado e das necessidades da organização.</span><span class="sxs-lookup"><span data-stu-id="37886-107">You can enroll organization-owned or corporate-owned devices to manage with Intune in a variety of ways, depending on the type of device, how the device was purchased, and the needs of the organization.</span></span> <span data-ttu-id="37886-108">Também é possível instalar o aplicativo Portal da Empresa para registrar e gerenciar dispositivos de propriedade corporativa, como em um cenário "traga seu próprio dispositivo" (BYOD).</span><span class="sxs-lookup"><span data-stu-id="37886-108">You also can install the Company Portal app to enroll and manage corporate-owned devices, like in a "bring your own device" (BYOD) scenario.</span></span>

<span data-ttu-id="37886-109">Os seguintes recursos do Graph estão disponíveis para gerenciar dispositivos corporativos no Intune:</span><span class="sxs-lookup"><span data-stu-id="37886-109">The following Graph resources are available to manage corporate-owned devices in Intune:</span></span>

- [<span data-ttu-id="37886-110">Perfil de implantação do Windows Autopilot do Active Directory</span><span class="sxs-lookup"><span data-stu-id="37886-110">Active directory windows autopilot deployment profile</span></span>](intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="37886-111">Perfil de implantação do Windows Autopilot do Azure AD</span><span class="sxs-lookup"><span data-stu-id="37886-111">Azure AD windows autopilot deployment profile</span></span>](intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="37886-112">Perfil básico de registro do DEP</span><span class="sxs-lookup"><span data-stu-id="37886-112">DEP enrollment base profile</span></span>](intune-enrollment-depenrollmentbaseprofile.md)
- [<span data-ttu-id="37886-113">Perfil de registro do DEP</span><span class="sxs-lookup"><span data-stu-id="37886-113">DEP enrollment profile</span></span>](intune-enrollment-depenrollmentprofile.md)
- [<span data-ttu-id="37886-114">Perfil de registro de iOS do DEP</span><span class="sxs-lookup"><span data-stu-id="37886-114">DEP iOS enrollment profile</span></span>](intune-enrollment-depiosenrollmentprofile.md)
- [<span data-ttu-id="37886-115">Perfil de registro de macOS do DEP</span><span class="sxs-lookup"><span data-stu-id="37886-115">DEP macOS enrollment profile</span></span>](intune-enrollment-depmacosenrollmentprofile.md)
- [<span data-ttu-id="37886-116">Configuração de integração do DEP</span><span class="sxs-lookup"><span data-stu-id="37886-116">DEP on-boarding setting</span></span>](intune-enrollment-deponboardingsetting.md)
- [<span data-ttu-id="37886-117">Tipo de token do DEP</span><span class="sxs-lookup"><span data-stu-id="37886-117">DEP token type</span></span>](intune-enrollment-deptokentype.md)
- [<span data-ttu-id="37886-118">Fonte de descoberta</span><span class="sxs-lookup"><span data-stu-id="37886-118">Discovery source</span></span>](intune-enrollment-discoverysource.md)
- [<span data-ttu-id="37886-119">Perfil de registro</span><span class="sxs-lookup"><span data-stu-id="37886-119">Enrollment profile</span></span>](intune-enrollment-enrollmentprofile.md)
- [<span data-ttu-id="37886-120">Estado de registro</span><span class="sxs-lookup"><span data-stu-id="37886-120">Enrollment state</span></span>](intune-enrollment-enrollmentstate.md)
- [<span data-ttu-id="37886-121">Identidade do dispositivo Apple importada</span><span class="sxs-lookup"><span data-stu-id="37886-121">Imported Apple device identity</span></span>](intune-enrollment-importedappledeviceidentity.md)
- [<span data-ttu-id="37886-122">Importar resultado de identidade do dispositivo Apple</span><span class="sxs-lookup"><span data-stu-id="37886-122">Imported Apple device identity result</span></span>](intune-enrollment-importedappledeviceidentityresult.md)
- [<span data-ttu-id="37886-123">Identidade do dispositivo importada</span><span class="sxs-lookup"><span data-stu-id="37886-123">Imported device identity</span></span>](intune-enrollment-importeddeviceidentity.md)
- [<span data-ttu-id="37886-124">Resultado de identidade do dispositivo importada</span><span class="sxs-lookup"><span data-stu-id="37886-124">Imported device identity result</span></span>](intune-enrollment-importeddeviceidentityresult.md)
- [<span data-ttu-id="37886-125">Tipo de identidade do dispositivo importada</span><span class="sxs-lookup"><span data-stu-id="37886-125">Imported device identity type</span></span>](intune-enrollment-importeddeviceidentitytype.md)
- [<span data-ttu-id="37886-126">Identidade importada do dispositivo do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="37886-126">Imported windows autopilot device identity</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentity.md)
- [<span data-ttu-id="37886-127">Status de importação da identidade de dispositivo importada do windows autopilot</span><span class="sxs-lookup"><span data-stu-id="37886-127">Imported windows autopilot device identity import status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)
- [<span data-ttu-id="37886-128">Estado de identidade de dispositivo importado do windows autopilot</span><span class="sxs-lookup"><span data-stu-id="37886-128">Imported windows autopilot device identity state</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)
- [<span data-ttu-id="37886-129">Carregar identidade de dispositivo importado do windows autopilot</span><span class="sxs-lookup"><span data-stu-id="37886-129">Imported windows autopilot device identity upload</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)
- [<span data-ttu-id="37886-130">Status de carregamento da identidade de dispositivo importado do windows autopilot</span><span class="sxs-lookup"><span data-stu-id="37886-130">Imported windows autopilot device identity upload status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)
- [<span data-ttu-id="37886-131">Modo de emparelhamento do iTunes</span><span class="sxs-lookup"><span data-stu-id="37886-131">iTunes pairing mode</span></span>](intune-enrollment-itunespairingmode.md)
- [<span data-ttu-id="37886-132">Certificado de gerenciamento com impressão digital</span><span class="sxs-lookup"><span data-stu-id="37886-132">Management certificate with thumbprint</span></span>](intune-enrollment-managementcertificatewiththumbprint.md)
- [<span data-ttu-id="37886-133">Configurações de experiência iniciais</span><span class="sxs-lookup"><span data-stu-id="37886-133">Out of box experience settings</span></span>](intune-enrollment-outofboxexperiencesettings.md)
- [<span data-ttu-id="37886-134">Plataforma</span><span class="sxs-lookup"><span data-stu-id="37886-134">Platform</span></span>](intune-enrollment-platform.md)
- [<span data-ttu-id="37886-135">Perfil de implantação do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="37886-135">Windows autopilot deployment profile</span></span>](intune-enrollment-windowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="37886-136">Atribuição do perfil de implantação do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="37886-136">Windows autopilot deployment profile assignment</span></span>](intune-enrollment-windowsautopilotdeploymentprofileassignment.md)
- [<span data-ttu-id="37886-137">Identidade do dispositivo do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="37886-137">Windows autopilot device identity</span></span>](intune-enrollment-windowsautopilotdeviceidentity.md)
- [<span data-ttu-id="37886-138">Status detalhado de atribuição do perfil do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="37886-138">Windows autopilot profile assignment detailed status</span></span>](intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)
- [<span data-ttu-id="37886-139">Status de atribuição do perfil do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="37886-139">Windows autopilot profile assignment status</span></span>](intune-enrollment-windowsautopilotprofileassignmentstatus.md)
- [<span data-ttu-id="37886-140">Configurações do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="37886-140">Windows autopilot settings</span></span>](intune-enrollment-windowsautopilotsettings.md)
- [<span data-ttu-id="37886-141">Status de sincronização do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="37886-141">Windows autopilot sync status</span></span>](intune-enrollment-windowsautopilotsyncstatus.md)
- [<span data-ttu-id="37886-142">Tipo de uso do dispositivo Windows</span><span class="sxs-lookup"><span data-stu-id="37886-142">Windows device usage type</span></span>](intune-enrollment-windowsdeviceusagetype.md)
- [<span data-ttu-id="37886-143">Configurações de tela de status de registro do Windows</span><span class="sxs-lookup"><span data-stu-id="37886-143">Windows enrollment status screen settings</span></span>](intune-enrollment-windowsenrollmentstatusscreensettings.md)
- [<span data-ttu-id="37886-144">Tipo de usuário do Windows</span><span class="sxs-lookup"><span data-stu-id="37886-144">Windows user type</span></span>](intune-enrollment-windowsusertype.md)
