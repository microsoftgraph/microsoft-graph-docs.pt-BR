---
title: Registrar dispositivos corporativos usando o Intune-Microsoft Graph API
description: Lista a API do Microsoft Graph para os pontos de extremidade do Intune (REST) que registram dispositivos para uma organização de locatário.
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 506f85ae59330757f4c6f12cf80795c6678b125e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36366368"
---
# <a name="enroll-corporate-owned-devices-by-using-intune"></a><span data-ttu-id="63525-103">Registrar dispositivos de propriedade corporativa por meio do Intune</span><span class="sxs-lookup"><span data-stu-id="63525-103">Enroll corporate-owned devices by using Intune</span></span>

> <span data-ttu-id="63525-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="63525-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="63525-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="63525-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="63525-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="63525-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63525-107">É possível registrar dispositivos pertencentes à organização ou de propriedade corporativa para serem gerenciados com o Intune de várias maneiras, dependendo do tipo de dispositivo, de como o dispositivo foi comprado e das necessidades da organização.</span><span class="sxs-lookup"><span data-stu-id="63525-107">You can enroll organization-owned or corporate-owned devices to manage with Intune in a variety of ways, depending on the type of device, how the device was purchased, and the needs of the organization.</span></span> <span data-ttu-id="63525-108">Também é possível instalar o aplicativo Portal da Empresa para registrar e gerenciar dispositivos de propriedade corporativa, como em um cenário "traga seu próprio dispositivo" (BYOD).</span><span class="sxs-lookup"><span data-stu-id="63525-108">You also can install the Company Portal app to enroll and manage corporate-owned devices, like in a "bring your own device" (BYOD) scenario.</span></span>

<span data-ttu-id="63525-109">Os seguintes recursos do Graph estão disponíveis para gerenciar dispositivos corporativos no Intune:</span><span class="sxs-lookup"><span data-stu-id="63525-109">The following Graph resources are available to manage corporate-owned devices in Intune:</span></span>

- [<span data-ttu-id="63525-110">Perfil de implantação do Windows Autopilot do Active Directory</span><span class="sxs-lookup"><span data-stu-id="63525-110">Active directory windows autopilot deployment profile</span></span>](intune-enrollment-activedirectorywindowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="63525-111">Perfil de implantação do Windows Autopilot do Azure AD</span><span class="sxs-lookup"><span data-stu-id="63525-111">Azure AD windows autopilot deployment profile</span></span>](intune-enrollment-azureadwindowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="63525-112">Perfil básico de registro do DEP</span><span class="sxs-lookup"><span data-stu-id="63525-112">DEP enrollment base profile</span></span>](intune-enrollment-depenrollmentbaseprofile.md)
- [<span data-ttu-id="63525-113">Perfil de registro do DEP</span><span class="sxs-lookup"><span data-stu-id="63525-113">DEP enrollment profile</span></span>](intune-enrollment-depenrollmentprofile.md)
- [<span data-ttu-id="63525-114">Perfil de registro de iOS do DEP</span><span class="sxs-lookup"><span data-stu-id="63525-114">DEP iOS enrollment profile</span></span>](intune-enrollment-depiosenrollmentprofile.md)
- [<span data-ttu-id="63525-115">Perfil de registro de macOS do DEP</span><span class="sxs-lookup"><span data-stu-id="63525-115">DEP macOS enrollment profile</span></span>](intune-enrollment-depmacosenrollmentprofile.md)
- [<span data-ttu-id="63525-116">Configuração de integração do DEP</span><span class="sxs-lookup"><span data-stu-id="63525-116">DEP on-boarding setting</span></span>](intune-enrollment-deponboardingsetting.md)
- [<span data-ttu-id="63525-117">Tipo de token do DEP</span><span class="sxs-lookup"><span data-stu-id="63525-117">DEP token type</span></span>](intune-enrollment-deptokentype.md)
- [<span data-ttu-id="63525-118">Fonte de descoberta</span><span class="sxs-lookup"><span data-stu-id="63525-118">Discovery source</span></span>](intune-enrollment-discoverysource.md)
- [<span data-ttu-id="63525-119">Perfil de registro</span><span class="sxs-lookup"><span data-stu-id="63525-119">Enrollment profile</span></span>](intune-enrollment-enrollmentprofile.md)
- [<span data-ttu-id="63525-120">Estado de registro</span><span class="sxs-lookup"><span data-stu-id="63525-120">Enrollment state</span></span>](intune-enrollment-enrollmentstate.md)
- [<span data-ttu-id="63525-121">Identidade do dispositivo Apple importada</span><span class="sxs-lookup"><span data-stu-id="63525-121">Imported Apple device identity</span></span>](intune-enrollment-importedappledeviceidentity.md)
- [<span data-ttu-id="63525-122">Importar resultado de identidade do dispositivo Apple</span><span class="sxs-lookup"><span data-stu-id="63525-122">Imported Apple device identity result</span></span>](intune-enrollment-importedappledeviceidentityresult.md)
- [<span data-ttu-id="63525-123">Identidade do dispositivo importada</span><span class="sxs-lookup"><span data-stu-id="63525-123">Imported device identity</span></span>](intune-enrollment-importeddeviceidentity.md)
- [<span data-ttu-id="63525-124">Resultado de identidade do dispositivo importada</span><span class="sxs-lookup"><span data-stu-id="63525-124">Imported device identity result</span></span>](intune-enrollment-importeddeviceidentityresult.md)
- [<span data-ttu-id="63525-125">Tipo de identidade do dispositivo importada</span><span class="sxs-lookup"><span data-stu-id="63525-125">Imported device identity type</span></span>](intune-enrollment-importeddeviceidentitytype.md)
- [<span data-ttu-id="63525-126">Identidade importada do dispositivo do Windows autopilot</span><span class="sxs-lookup"><span data-stu-id="63525-126">Imported windows autopilot device identity</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentity.md)
- [<span data-ttu-id="63525-127">Status de importação da identidade de dispositivo importada do windows autopilot</span><span class="sxs-lookup"><span data-stu-id="63525-127">Imported windows autopilot device identity import status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityimportstatus.md)
- [<span data-ttu-id="63525-128">Estado de identidade de dispositivo importado do windows autopilot</span><span class="sxs-lookup"><span data-stu-id="63525-128">Imported windows autopilot device identity state</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentitystate.md)
- [<span data-ttu-id="63525-129">Status de carregamento da identidade de dispositivo importado do windows autopilot</span><span class="sxs-lookup"><span data-stu-id="63525-129">Imported windows autopilot device identity upload status</span></span>](intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)
- [<span data-ttu-id="63525-130">Modo de emparelhamento do iTunes</span><span class="sxs-lookup"><span data-stu-id="63525-130">iTunes pairing mode</span></span>](intune-enrollment-itunespairingmode.md)
- [<span data-ttu-id="63525-131">Certificado de gerenciamento com impressão digital</span><span class="sxs-lookup"><span data-stu-id="63525-131">Management certificate with thumbprint</span></span>](intune-enrollment-managementcertificatewiththumbprint.md)
- [<span data-ttu-id="63525-132">Configurações de experiência iniciais</span><span class="sxs-lookup"><span data-stu-id="63525-132">Out of box experience settings</span></span>](intune-enrollment-outofboxexperiencesettings.md)
- [<span data-ttu-id="63525-133">Plataforma</span><span class="sxs-lookup"><span data-stu-id="63525-133">Platform</span></span>](intune-enrollment-platform.md)
- [<span data-ttu-id="63525-134">Perfil de implantação do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="63525-134">Windows autopilot deployment profile</span></span>](intune-enrollment-windowsautopilotdeploymentprofile.md)
- [<span data-ttu-id="63525-135">Atribuição do perfil de implantação do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="63525-135">Windows autopilot deployment profile assignment</span></span>](intune-enrollment-windowsautopilotdeploymentprofileassignment.md)
- [<span data-ttu-id="63525-136">Identidade do dispositivo do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="63525-136">Windows autopilot device identity</span></span>](intune-enrollment-windowsautopilotdeviceidentity.md)
- [<span data-ttu-id="63525-137">Tipo de dispositivo do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="63525-137">Windows autopilot device type</span></span>](intune-enrollment-windowsautopilotdevicetype.md)
- [<span data-ttu-id="63525-138">Status detalhado de atribuição do perfil do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="63525-138">Windows autopilot profile assignment detailed status</span></span>](intune-enrollment-windowsautopilotprofileassignmentdetailedstatus.md)
- [<span data-ttu-id="63525-139">Status de atribuição do perfil do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="63525-139">Windows autopilot profile assignment status</span></span>](intune-enrollment-windowsautopilotprofileassignmentstatus.md)
- [<span data-ttu-id="63525-140">Configurações do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="63525-140">Windows autopilot settings</span></span>](intune-enrollment-windowsautopilotsettings.md)
- [<span data-ttu-id="63525-141">Status de sincronização do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="63525-141">Windows autopilot sync status</span></span>](intune-enrollment-windowsautopilotsyncstatus.md)
- [<span data-ttu-id="63525-142">Tipo de uso do dispositivo Windows</span><span class="sxs-lookup"><span data-stu-id="63525-142">Windows device usage type</span></span>](intune-enrollment-windowsdeviceusagetype.md)
- [<span data-ttu-id="63525-143">Configurações de tela de status de registro do Windows</span><span class="sxs-lookup"><span data-stu-id="63525-143">Windows enrollment status screen settings</span></span>](intune-enrollment-windowsenrollmentstatusscreensettings.md)
- [<span data-ttu-id="63525-144">Tipo de usuário do Windows</span><span class="sxs-lookup"><span data-stu-id="63525-144">Windows user type</span></span>](intune-enrollment-windowsusertype.md)
