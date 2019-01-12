---
title: Gerenciamento de dispositivos no Microsoft Intune
description: ''
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3d665b70f812a18f840ce43a029fe0729d454745
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980640"
---
# <a name="device-management-in-microsoft-intune"></a><span data-ttu-id="cefbf-102">Gerenciamento de dispositivos no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="cefbf-102">Device management in Microsoft Intune</span></span>

> <span data-ttu-id="cefbf-103">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="cefbf-103">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

- [<span data-ttu-id="cefbf-104">Estado de ação</span><span class="sxs-lookup"><span data-stu-id="cefbf-104">Action state</span></span>](intune-devices-actionstate.md)
- [<span data-ttu-id="cefbf-105">Certificado de notificação por push da Apple</span><span class="sxs-lookup"><span data-stu-id="cefbf-105">Apple push notification certificate</span></span>](intune-devices-applepushnotificationcertificate.md)
- [<span data-ttu-id="cefbf-106">Ator de auditoria</span><span class="sxs-lookup"><span data-stu-id="cefbf-106">Audit actor</span></span>](intune-auditing-auditactor.md)
- [<span data-ttu-id="cefbf-107">Evento de auditoria</span><span class="sxs-lookup"><span data-stu-id="cefbf-107">Audit event</span></span>](intune-auditing-auditevent.md)
- [<span data-ttu-id="cefbf-108">Propriedade de auditoria</span><span class="sxs-lookup"><span data-stu-id="cefbf-108">Audit property</span></span>](intune-auditing-auditproperty.md)
- [<span data-ttu-id="cefbf-109">Recurso de auditoria</span><span class="sxs-lookup"><span data-stu-id="cefbf-109">Audit resource</span></span>](intune-auditing-auditresource.md)
- [<span data-ttu-id="cefbf-110">Estado de conformidade</span><span class="sxs-lookup"><span data-stu-id="cefbf-110">Compliance state</span></span>](intune-devices-compliancestate.md)
- [<span data-ttu-id="cefbf-111">Recursos habilitados pelo cliente do Gerenciador de Configurações</span><span class="sxs-lookup"><span data-stu-id="cefbf-111">Configuration manager client enabled features</span></span>](intune-devices-configurationmanagerclientenabledfeatures.md)
- [<span data-ttu-id="cefbf-112">Resultado da ação de excluir o usuário do dispositivo compartilhado da Apple</span><span class="sxs-lookup"><span data-stu-id="cefbf-112">Delete user from shared Apple device action result</span></span>](intune-devices-deleteuserfromsharedappledeviceactionresult.md)
- [<span data-ttu-id="cefbf-113">Aplicativo detectado</span><span class="sxs-lookup"><span data-stu-id="cefbf-113">Detected app</span></span>](intune-devices-detectedapp.md)
- [<span data-ttu-id="cefbf-114">Resultado da ação do dispositivo</span><span class="sxs-lookup"><span data-stu-id="cefbf-114">Device action result</span></span>](intune-devices-deviceactionresult.md)
- [<span data-ttu-id="cefbf-115">Motivo da falha do dispositivo inscrição</span><span class="sxs-lookup"><span data-stu-id="cefbf-115">Device enrollment failure reason</span></span>](intune-troubleshooting-deviceenrollmentfailurereason.md)
- [<span data-ttu-id="cefbf-116">Tipo de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="cefbf-116">Device enrollment type</span></span>](intune-devices-deviceenrollmenttype.md)
- [<span data-ttu-id="cefbf-117">Resumo do Estado de Acesso ao Exchange do dispositivo</span><span class="sxs-lookup"><span data-stu-id="cefbf-117">Device exchange access state summary</span></span>](intune-devices-deviceexchangeaccessstatesummary.md)
- [<span data-ttu-id="cefbf-118">Geolocalização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="cefbf-118">Device geolocation</span></span>](intune-devices-devicegeolocation.md)
- [<span data-ttu-id="cefbf-119">Estado do atestado de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="cefbf-119">Device health attestation state</span></span>](intune-devices-devicehealthattestationstate.md)
- [<span data-ttu-id="cefbf-120">Estado de acesso do exchange de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="cefbf-120">Device management exchange access state</span></span>](intune-devices-devicemanagementexchangeaccessstate.md)
- [<span data-ttu-id="cefbf-121">Motivo de estado de acesso do dispositivo gerenciamento exchange</span><span class="sxs-lookup"><span data-stu-id="cefbf-121">Device management exchange access state reason</span></span>](intune-devices-devicemanagementexchangeaccessstatereason.md)
- [<span data-ttu-id="cefbf-122">Estado de assinatura do gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="cefbf-122">Device management subscription state</span></span>](intune-devices-devicemanagementsubscriptionstate.md)
- [<span data-ttu-id="cefbf-123">Evento de solução de problemas com o gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="cefbf-123">Device management troubleshooting event</span></span>](intune-troubleshooting-devicemanagementtroubleshootingevent.md)
- [<span data-ttu-id="cefbf-124">Resumo do sistema operacional do dispositivo</span><span class="sxs-lookup"><span data-stu-id="cefbf-124">Device operating system summary</span></span>](intune-devices-deviceoperatingsystemsummary.md)
- [<span data-ttu-id="cefbf-125">Estado do registro de dispositivo</span><span class="sxs-lookup"><span data-stu-id="cefbf-125">Device registration state</span></span>](intune-devices-deviceregistrationstate.md)
- [<span data-ttu-id="cefbf-126">Evento de solução de problemas de registro</span><span class="sxs-lookup"><span data-stu-id="cefbf-126">Enrollment troubleshooting event</span></span>](intune-troubleshooting-enrollmenttroubleshootingevent.md)
- [<span data-ttu-id="cefbf-127">Mensagem de notificação localizada</span><span class="sxs-lookup"><span data-stu-id="cefbf-127">Localized notification message</span></span>](intune-notification-localizednotificationmessage.md)
- [<span data-ttu-id="cefbf-128">Resultado da ação de localizar dispositivo</span><span class="sxs-lookup"><span data-stu-id="cefbf-128">Locate device action result</span></span>](intune-devices-locatedeviceactionresult.md)
- [<span data-ttu-id="cefbf-129">Dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="cefbf-129">Managed device</span></span>](intune-devices-manageddevice.md)
- [<span data-ttu-id="cefbf-130">Visão geral do dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="cefbf-130">Managed device overview</span></span>](intune-devices-manageddeviceoverview.md)
- [<span data-ttu-id="cefbf-131">Tipo de proprietário do dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="cefbf-131">Managed device owner type</span></span>](intune-devices-manageddeviceownertype.md)
- [<span data-ttu-id="cefbf-132">Parceria de dispositivo gerenciado relatou o estado de integridade</span><span class="sxs-lookup"><span data-stu-id="cefbf-132">Managed device partner reported health state</span></span>](intune-devices-manageddevicepartnerreportedhealthstate.md)
- [<span data-ttu-id="cefbf-133">Tipo de agente de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="cefbf-133">Management agent type</span></span>](intune-devices-managementagenttype.md)
- [<span data-ttu-id="cefbf-134">Modelo de mensagem de notificação</span><span class="sxs-lookup"><span data-stu-id="cefbf-134">Notification message template</span></span>](intune-notification-notificationmessagetemplate.md)
- [<span data-ttu-id="cefbf-135">Opções de identidade visual do modelo de notificação</span><span class="sxs-lookup"><span data-stu-id="cefbf-135">Notification template branding options</span></span>](intune-notification-notificationtemplatebrandingoptions.md)
- [<span data-ttu-id="cefbf-136">Status de nível de contratação da assistência remota</span><span class="sxs-lookup"><span data-stu-id="cefbf-136">Remote assistance on-boarding status</span></span>](intune-remoteassistance-remoteassistanceonboardingstatus.md)
- [<span data-ttu-id="cefbf-137">Parceiro de assistência remota</span><span class="sxs-lookup"><span data-stu-id="cefbf-137">Remote assistance partner</span></span>](intune-remoteassistance-remoteassistancepartner.md)
- [<span data-ttu-id="cefbf-138">Resultado da ação de bloqueio remoto</span><span class="sxs-lookup"><span data-stu-id="cefbf-138">Remote lock action result</span></span>](intune-devices-remotelockactionresult.md)
- [<span data-ttu-id="cefbf-139">Resultado da ação de redefinir a senha</span><span class="sxs-lookup"><span data-stu-id="cefbf-139">Reset passcode action result</span></span>](intune-devices-resetpasscodeactionresult.md)
- [<span data-ttu-id="cefbf-140">Parâmetro da ação de atualização de conta de dispositivo Windows</span><span class="sxs-lookup"><span data-stu-id="cefbf-140">Update windows device account action parameter</span></span>](intune-devices-updatewindowsdeviceaccountactionparameter.md)
- [<span data-ttu-id="cefbf-141">Resultado da ação de verificação do Windows Defender</span><span class="sxs-lookup"><span data-stu-id="cefbf-141">Windows defender scan action result</span></span>](intune-devices-windowsdefenderscanactionresult.md)
- [<span data-ttu-id="cefbf-142">Conta do dispositivo Windows</span><span class="sxs-lookup"><span data-stu-id="cefbf-142">Windows device account</span></span>](intune-devices-windowsdeviceaccount.md)
- [<span data-ttu-id="cefbf-143">Conta do AD de dispositivo Windows</span><span class="sxs-lookup"><span data-stu-id="cefbf-143">Windows device AD account</span></span>](intune-devices-windowsdeviceadaccount.md)
- [<span data-ttu-id="cefbf-144">Conta do Azure AD de dispositivo Windows</span><span class="sxs-lookup"><span data-stu-id="cefbf-144">Windows device Azure AD account</span></span>](intune-devices-windowsdeviceazureadaccount.md)
