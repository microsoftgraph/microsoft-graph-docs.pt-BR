---
title: Gerenciamento de dispositivos no Microsoft Intune
description: ''
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4c8f6676647405e8186e9d27466266f6690e2cd1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575230"
---
# <a name="device-management-in-microsoft-intune"></a><span data-ttu-id="5e63d-102">Gerenciamento de dispositivos no Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="5e63d-102">Device management in Microsoft Intune</span></span>

> <span data-ttu-id="5e63d-103">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5e63d-103">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

- [<span data-ttu-id="5e63d-104">Estado da ação</span><span class="sxs-lookup"><span data-stu-id="5e63d-104">Action state</span></span>](intune-devices-actionstate.md)
- [<span data-ttu-id="5e63d-105">Certificado de notificação por push da Apple</span><span class="sxs-lookup"><span data-stu-id="5e63d-105">Apple push notification certificate</span></span>](intune-devices-applepushnotificationcertificate.md)
- [<span data-ttu-id="5e63d-106">Ator de auditoria</span><span class="sxs-lookup"><span data-stu-id="5e63d-106">Audit actor</span></span>](intune-auditing-auditactor.md)
- [<span data-ttu-id="5e63d-107">Evento de auditoria</span><span class="sxs-lookup"><span data-stu-id="5e63d-107">Audit event</span></span>](intune-auditing-auditevent.md)
- [<span data-ttu-id="5e63d-108">Propriedade de auditoria</span><span class="sxs-lookup"><span data-stu-id="5e63d-108">Audit property</span></span>](intune-auditing-auditproperty.md)
- [<span data-ttu-id="5e63d-109">Recurso de auditoria</span><span class="sxs-lookup"><span data-stu-id="5e63d-109">Audit resource</span></span>](intune-auditing-auditresource.md)
- [<span data-ttu-id="5e63d-110">Estado de conformidade</span><span class="sxs-lookup"><span data-stu-id="5e63d-110">Compliance state</span></span>](intune-devices-compliancestate.md)
- [<span data-ttu-id="5e63d-111">Recursos habilitados pelo cliente do Gerenciador de Configurações</span><span class="sxs-lookup"><span data-stu-id="5e63d-111">Configuration manager client enabled features</span></span>](intune-devices-configurationmanagerclientenabledfeatures.md)
- [<span data-ttu-id="5e63d-112">Resultado da ação de excluir o usuário do dispositivo compartilhado da Apple</span><span class="sxs-lookup"><span data-stu-id="5e63d-112">Delete user from shared Apple device action result</span></span>](intune-devices-deleteuserfromsharedappledeviceactionresult.md)
- [<span data-ttu-id="5e63d-113">Aplicativo detectado</span><span class="sxs-lookup"><span data-stu-id="5e63d-113">Detected app</span></span>](intune-devices-detectedapp.md)
- [<span data-ttu-id="5e63d-114">Resultado da ação do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5e63d-114">Device action result</span></span>](intune-devices-deviceactionresult.md)
- [<span data-ttu-id="5e63d-115">Motivo da falha de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5e63d-115">Device enrollment failure reason</span></span>](intune-troubleshooting-deviceenrollmentfailurereason.md)
- [<span data-ttu-id="5e63d-116">Resumo do Estado de Acesso ao Exchange do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5e63d-116">Device exchange access state summary</span></span>](intune-devices-deviceexchangeaccessstatesummary.md)
- [<span data-ttu-id="5e63d-117">Geolocalização do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5e63d-117">Device geolocation</span></span>](intune-devices-devicegeolocation.md)
- [<span data-ttu-id="5e63d-118">Estado do atestado de integridade do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5e63d-118">Device health attestation state</span></span>](intune-devices-devicehealthattestationstate.md)
- [<span data-ttu-id="5e63d-119">Estado de acesso do Exchange de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="5e63d-119">Device management exchange access state</span></span>](intune-devices-devicemanagementexchangeaccessstate.md)
- [<span data-ttu-id="5e63d-120">Motivo do estado de acesso do Exchange de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="5e63d-120">Device management exchange access state reason</span></span>](intune-devices-devicemanagementexchangeaccessstatereason.md)
- [<span data-ttu-id="5e63d-121">Estado de assinatura de gerenciamento de dispositivo</span><span class="sxs-lookup"><span data-stu-id="5e63d-121">Device management subscription state</span></span>](intune-devices-devicemanagementsubscriptionstate.md)
- [<span data-ttu-id="5e63d-122">Evento de solução de problemas com o gerenciamento de dispositivos</span><span class="sxs-lookup"><span data-stu-id="5e63d-122">Device management troubleshooting event</span></span>](intune-troubleshooting-devicemanagementtroubleshootingevent.md)
- [<span data-ttu-id="5e63d-123">Resumo do sistema operacional do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5e63d-123">Device operating system summary</span></span>](intune-devices-deviceoperatingsystemsummary.md)
- [<span data-ttu-id="5e63d-124">Estado do registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="5e63d-124">Device registration state</span></span>](intune-devices-deviceregistrationstate.md)
- [<span data-ttu-id="5e63d-125">Evento de solução de problemas de registro</span><span class="sxs-lookup"><span data-stu-id="5e63d-125">Enrollment troubleshooting event</span></span>](intune-troubleshooting-enrollmenttroubleshootingevent.md)
- [<span data-ttu-id="5e63d-126">Mensagem de notificação localizada</span><span class="sxs-lookup"><span data-stu-id="5e63d-126">Localized notification message</span></span>](intune-notification-localizednotificationmessage.md)
- [<span data-ttu-id="5e63d-127">Resultado da ação de localizar dispositivo</span><span class="sxs-lookup"><span data-stu-id="5e63d-127">Locate device action result</span></span>](intune-devices-locatedeviceactionresult.md)
- [<span data-ttu-id="5e63d-128">Dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="5e63d-128">Managed device</span></span>](intune-devices-manageddevice.md)
- [<span data-ttu-id="5e63d-129">Visão geral do dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="5e63d-129">Managed device overview</span></span>](intune-devices-manageddeviceoverview.md)
- [<span data-ttu-id="5e63d-130">Tipo de proprietário do dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="5e63d-130">Managed device owner type</span></span>](intune-devices-manageddeviceownertype.md)
- [<span data-ttu-id="5e63d-131">Estado de integridade reportado pelo parceiro do dispositivo gerenciado</span><span class="sxs-lookup"><span data-stu-id="5e63d-131">Managed device partner reported health state</span></span>](intune-devices-manageddevicepartnerreportedhealthstate.md)
- [<span data-ttu-id="5e63d-132">Tipo de agente de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="5e63d-132">Management agent type</span></span>](intune-devices-managementagenttype.md)
- [<span data-ttu-id="5e63d-133">Modelo de mensagem de notificação</span><span class="sxs-lookup"><span data-stu-id="5e63d-133">Notification message template</span></span>](intune-notification-notificationmessagetemplate.md)
- [<span data-ttu-id="5e63d-134">Opções de identidade visual do modelo de notificação</span><span class="sxs-lookup"><span data-stu-id="5e63d-134">Notification template branding options</span></span>](intune-notification-notificationtemplatebrandingoptions.md)
- [<span data-ttu-id="5e63d-135">Status da inclusão de assistência remota</span><span class="sxs-lookup"><span data-stu-id="5e63d-135">Remote assistance on-boarding status</span></span>](intune-remoteassistance-remoteassistanceonboardingstatus.md)
- [<span data-ttu-id="5e63d-136">Parceiro de assistência remota</span><span class="sxs-lookup"><span data-stu-id="5e63d-136">Remote assistance partner</span></span>](intune-remoteassistance-remoteassistancepartner.md)
- [<span data-ttu-id="5e63d-137">Resultado da ação de bloqueio remoto</span><span class="sxs-lookup"><span data-stu-id="5e63d-137">Remote lock action result</span></span>](intune-devices-remotelockactionresult.md)
- [<span data-ttu-id="5e63d-138">Resultado da ação de redefinir a senha</span><span class="sxs-lookup"><span data-stu-id="5e63d-138">Reset passcode action result</span></span>](intune-devices-resetpasscodeactionresult.md)
- [<span data-ttu-id="5e63d-139">Parâmetro da ação de atualização de conta de dispositivo Windows</span><span class="sxs-lookup"><span data-stu-id="5e63d-139">Update windows device account action parameter</span></span>](intune-devices-updatewindowsdeviceaccountactionparameter.md)
- [<span data-ttu-id="5e63d-140">Resultado da ação de verificação do Windows Defender</span><span class="sxs-lookup"><span data-stu-id="5e63d-140">Windows defender scan action result</span></span>](intune-devices-windowsdefenderscanactionresult.md)
- [<span data-ttu-id="5e63d-141">Conta do dispositivo Windows</span><span class="sxs-lookup"><span data-stu-id="5e63d-141">Windows device account</span></span>](intune-devices-windowsdeviceaccount.md)
- [<span data-ttu-id="5e63d-142">Conta do AD de dispositivo Windows</span><span class="sxs-lookup"><span data-stu-id="5e63d-142">Windows device AD account</span></span>](intune-devices-windowsdeviceadaccount.md)
- [<span data-ttu-id="5e63d-143">Conta do Azure AD de dispositivo Windows</span><span class="sxs-lookup"><span data-stu-id="5e63d-143">Windows device Azure AD account</span></span>](intune-devices-windowsdeviceazureadaccount.md)
