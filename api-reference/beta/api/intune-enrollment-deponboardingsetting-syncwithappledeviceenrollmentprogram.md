---
title: ação de syncWithAppleDeviceEnrollmentProgram
description: Sincroniza entre Intune e o programa de inscrição do dispositivo Apple
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c6e13a9f245f7ca2a1ac197181fd82e6504e44f2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812343"
---
# <a name="syncwithappledeviceenrollmentprogram-action"></a><span data-ttu-id="a0472-103">ação de syncWithAppleDeviceEnrollmentProgram</span><span class="sxs-lookup"><span data-stu-id="a0472-103">syncWithAppleDeviceEnrollmentProgram action</span></span>

> <span data-ttu-id="a0472-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a0472-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a0472-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a0472-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a0472-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a0472-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a0472-107">Sincroniza entre Intune e o programa de inscrição do dispositivo Apple</span><span class="sxs-lookup"><span data-stu-id="a0472-107">Synchronizes between Apple Device Enrollment Program and Intune</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a0472-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a0472-108">Prerequisites</span></span>
<span data-ttu-id="a0472-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a0472-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0472-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a0472-111">Permission type</span></span>|<span data-ttu-id="a0472-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a0472-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0472-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a0472-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a0472-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0472-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a0472-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a0472-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0472-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0472-116">Not supported.</span></span>|
|<span data-ttu-id="a0472-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a0472-117">Application</span></span>|<span data-ttu-id="a0472-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a0472-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0472-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a0472-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/syncWithAppleDeviceEnrollmentProgram
```

## <a name="request-headers"></a><span data-ttu-id="a0472-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a0472-120">Request headers</span></span>
|<span data-ttu-id="a0472-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a0472-121">Header</span></span>|<span data-ttu-id="a0472-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a0472-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0472-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a0472-123">Authorization</span></span>|<span data-ttu-id="a0472-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a0472-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0472-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a0472-125">Accept</span></span>|<span data-ttu-id="a0472-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a0472-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0472-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a0472-127">Request body</span></span>
<span data-ttu-id="a0472-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a0472-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a0472-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0472-129">Response</span></span>
<span data-ttu-id="a0472-130">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="a0472-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a0472-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a0472-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="a0472-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a0472-132">Request</span></span>
<span data-ttu-id="a0472-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a0472-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/syncWithAppleDeviceEnrollmentProgram
```

### <a name="response"></a><span data-ttu-id="a0472-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a0472-134">Response</span></span>
<span data-ttu-id="a0472-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a0472-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





