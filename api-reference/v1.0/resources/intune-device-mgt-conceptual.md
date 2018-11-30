---
title: Gerenciamento de dispositivos no Microsoft Intune
description: ''
ms.openlocfilehash: db7cc57a7f7b4463de494d49d4400cd7a563abaf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006499"
---
# <a name="device-management-in-microsoft-intune"></a><span data-ttu-id="9c500-102">Gerenciamento de dispositivos no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="9c500-102">Device management in Microsoft Intune</span></span>

> <span data-ttu-id="9c500-103">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9c500-103">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

- [<span data-ttu-id="9c500-104">Estado de ação</span><span class="sxs-lookup"><span data-stu-id="9c500-104">Action state</span></span>](intune-devices-actionstate.md)
- [<span data-ttu-id="9c500-105">Certificado de notificação por push da Apple</span><span class="sxs-lookup"><span data-stu-id="9c500-105">Apple push notification certificate</span></span>](intune-devices-applepushnotificationcertificate.md)
- [<span data-ttu-id="9c500-106">Ator de auditoria</span><span class="sxs-lookup"><span data-stu-id="9c500-106">Audit actor</span></span>](intune-auditing-auditactor.md)
- [<span data-ttu-id="9c500-107">Evento de auditoria</span><span class="sxs-lookup"><span data-stu-id="9c500-107">Audit event</span></span>](intune-auditing-auditevent.md)
- [<span data-ttu-id="9c500-108">Propriedade de auditoria</span><span class="sxs-lookup"><span data-stu-id="9c500-108">Audit property</span></span>](intune-auditing-auditproperty.md)
- [<span data-ttu-id="9c500-109">Recurso de auditoria</span><span class="sxs-lookup"><span data-stu-id="9c500-109">Audit resource</span></span>](intune-auditing-auditresource.md)
- [<span data-ttu-id="9c500-110">Estado de conformidade</span><span class="sxs-lookup"><span data-stu-id="9c500-110">Compliance state</span></span>](intune-devices-compliancestate.md)
- [<span data-ttu-id="9c500-111">Recursos habilitados pelo cliente do Gerenciador de Configurações</span><span class="sxs-lookup"><span data-stu-id="9c500-111">Configuration manager client enabled features</span></span>](intune-devices-configurationmanagerclientenabledfeatures.md)
- [<span data-ttu-id="9c500-112">Resultado da ação de excluir o usuário do dispositivo compartilhado da Apple</span><span class="sxs-lookup"><span data-stu-id="9c500-112">Delete user from shared Apple device action result</span></span>](intune-devices-deleteuserfromsharedappledeviceactionresult.md)
- [<span data-ttu-id="9c500-113">Aplicativo detectado</span><span class="sxs-lookup"><span data-stu-id="9c500-113">Detected app</span></span>](intune-devices-detectedapp.md)
- [<span data-ttu-id="9c500-114">Resultado da ação do dispositivo</span><span class="sxs-lookup"><span data-stu-id="9c500-114">Device action result</span></span>](intune-devices-deviceactionresult.md)
- [<span data-ttu-id="9c500-115">Motivo da falha do dispositivo inscrição</span><span class="sxs-lookup"><span data-stu-id="9c500-115">Device enrollment failure reason</span></span>](intune-troubleshooting-deviceenrollmentfailurereason.md)
- [<span data-ttu-id="9c500-116">Tipo de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="9c500-116">Device enrollment type</span></span>](intune-devices-deviceenrollmenttype.md)
- [<span data-ttu-id="9c500-117">Resumo do Estado de Acesso ao Exchange do dispositivo</span><span class="sxs-lookup"><span data-stu-id="9c500-117">Device exchange access state summary</span></span>](intune-devices-deviceexchangeaccessstatesummary.md)
- [<span data-ttu-id="9c500-118">Geolocalização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="9c500-118">Device geolocation</span></span>](intune-devices-devicegeolocation.md)
- [<span data-ttu-id="9c500-119">Estado do atestado de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="9c500-119">Device health attestation state</span></span>](intune-devices-devicehealthattestationstate.md)
- [<span data-ttu-id="9c500-120">Estado de acesso do exchange de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="9c500-120">Device management exchange access state</span></span>](intune-devices-devicemanagementexchangeaccessstate.md)
- [<span data-ttu-id="9c500-121">Motivo de estado de acesso do dispositivo gerenciamento exchange</span><span class="sxs-lookup"><span data-stu-id="9c500-121">Device management exchange access state reason</span></span>](intune-devices-devicemanagementexchangeaccessstatereason.md)
- [<span data-ttu-id="9c500-122">Estado de assinatura do gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="9c500-122">Device management subscription state</span></span>](intune-devices-devicemanagementsubscriptionstate.md)
- [<span data-ttu-id="9c500-123">Evento de solução de problemas com o gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="9c500-123">Device management troubleshooting event</span></span>](intune-troubleshooting-devicemanagementtroubleshootingevent.md)
- [<span data-ttu-id="9c500-124">Resumo do sistema operacional do dispositivo</span><span class="sxs-lookup"><span data-stu-id="9c500-124">Device operating system summary</span></span>](intune-devices-deviceoperatingsystemsummary.md)
- [<span data-ttu-id="9c500-125">Estado do registro de dispositivo</span><span class="sxs-lookup"><span data-stu-id="9c500-125">Device registration state</span></span>](intune-devices-deviceregistrationstate.md)
- [<span data-ttu-id="9c500-126">Evento de solução de problemas de registro</span><span class="sxs-lookup"><span data-stu-id="9c500-126">Enrollment troubleshooting event</span></span>](intune-troubleshooting-enrollmenttroubleshootingevent.md)
- [<span data-ttu-id="9c500-127">Mensagem de notificação localizada</span><span class="sxs-lookup"><span data-stu-id="9c500-127">Localized notification message</span></span>](intune-notification-localizednotificationmessage.md)
- [<span data-ttu-id="9c500-128">Resultado da ação de localizar dispositivo</span><span class="sxs-lookup"><span data-stu-id="9c500-128">Locate device action result</span></span>](intune-devices-locatedeviceactionresult.md)
- [<span data-ttu-id="9c500-129">Dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="9c500-129">Managed device</span></span>](intune-devices-manageddevice.md)
- [<span data-ttu-id="9c500-130">Visão geral do dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="9c500-130">Managed device overview</span></span>](intune-devices-manageddeviceoverview.md)
- [<span data-ttu-id="9c500-131">Tipo de proprietário do dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="9c500-131">Managed device owner type</span></span>](intune-devices-manageddeviceownertype.md)
- [<span data-ttu-id="9c500-132">Parceria de dispositivo gerenciado relatou o estado de integridade</span><span class="sxs-lookup"><span data-stu-id="9c500-132">Managed device partner reported health state</span></span>](intune-devices-manageddevicepartnerreportedhealthstate.md)
- [<span data-ttu-id="9c500-133">Tipo de agente de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="9c500-133">Management agent type</span></span>](intune-devices-managementagenttype.md)
- [<span data-ttu-id="9c500-134">Modelo de mensagem de notificação</span><span class="sxs-lookup"><span data-stu-id="9c500-134">Notification message template</span></span>](intune-notification-notificationmessagetemplate.md)
- [<span data-ttu-id="9c500-135">Opções de identidade visual do modelo de notificação</span><span class="sxs-lookup"><span data-stu-id="9c500-135">Notification template branding options</span></span>](intune-notification-notificationtemplatebrandingoptions.md)
- [<span data-ttu-id="9c500-136">Status de nível de contratação da assistência remota</span><span class="sxs-lookup"><span data-stu-id="9c500-136">Remote assistance on-boarding status</span></span>](intune-remoteassistance-remoteassistanceonboardingstatus.md)
- [<span data-ttu-id="9c500-137">Parceiro de assistência remota</span><span class="sxs-lookup"><span data-stu-id="9c500-137">Remote assistance partner</span></span>](intune-remoteassistance-remoteassistancepartner.md)
- [<span data-ttu-id="9c500-138">Resultado da ação de bloqueio remoto</span><span class="sxs-lookup"><span data-stu-id="9c500-138">Remote lock action result</span></span>](intune-devices-remotelockactionresult.md)
- [<span data-ttu-id="9c500-139">Resultado da ação de redefinir a senha</span><span class="sxs-lookup"><span data-stu-id="9c500-139">Reset passcode action result</span></span>](intune-devices-resetpasscodeactionresult.md)
- [<span data-ttu-id="9c500-140">Parâmetro da ação de atualização de conta de dispositivo Windows</span><span class="sxs-lookup"><span data-stu-id="9c500-140">Update windows device account action parameter</span></span>](intune-devices-updatewindowsdeviceaccountactionparameter.md)
- [<span data-ttu-id="9c500-141">Resultado da ação de verificação do Windows Defender</span><span class="sxs-lookup"><span data-stu-id="9c500-141">Windows defender scan action result</span></span>](intune-devices-windowsdefenderscanactionresult.md)
- [<span data-ttu-id="9c500-142">Conta do dispositivo Windows</span><span class="sxs-lookup"><span data-stu-id="9c500-142">Windows device account</span></span>](intune-devices-windowsdeviceaccount.md)
- [<span data-ttu-id="9c500-143">Conta do AD de dispositivo Windows</span><span class="sxs-lookup"><span data-stu-id="9c500-143">Windows device AD account</span></span>](intune-devices-windowsdeviceadaccount.md)
- [<span data-ttu-id="9c500-144">Conta do Azure AD de dispositivo Windows</span><span class="sxs-lookup"><span data-stu-id="9c500-144">Windows device Azure AD account</span></span>](intune-devices-windowsdeviceazureadaccount.md)
