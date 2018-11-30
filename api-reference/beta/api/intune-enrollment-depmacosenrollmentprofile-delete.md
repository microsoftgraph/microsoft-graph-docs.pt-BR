---
title: Excluir depMacOSEnrollmentProfile
description: Exclui um depMacOSEnrollmentProfile.
ms.openlocfilehash: 61b7ad694e5e8470ea2f66506d6b00de345b05fe
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034319"
---
# <a name="delete-depmacosenrollmentprofile"></a><span data-ttu-id="f0bbf-103">Excluir depMacOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="f0bbf-103">Delete depMacOSEnrollmentProfile</span></span>

> <span data-ttu-id="f0bbf-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f0bbf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f0bbf-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f0bbf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f0bbf-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f0bbf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f0bbf-107">Exclui um [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="f0bbf-107">Deletes a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f0bbf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f0bbf-108">Prerequisites</span></span>
<span data-ttu-id="f0bbf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0bbf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0bbf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0bbf-111">Permission type</span></span>|<span data-ttu-id="f0bbf-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f0bbf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0bbf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0bbf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f0bbf-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0bbf-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f0bbf-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0bbf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0bbf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0bbf-116">Not supported.</span></span>|
|<span data-ttu-id="f0bbf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0bbf-117">Application</span></span>|<span data-ttu-id="f0bbf-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0bbf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0bbf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f0bbf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="f0bbf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f0bbf-120">Request headers</span></span>
|<span data-ttu-id="f0bbf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f0bbf-121">Header</span></span>|<span data-ttu-id="f0bbf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f0bbf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0bbf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f0bbf-123">Authorization</span></span>|<span data-ttu-id="f0bbf-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0bbf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0bbf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f0bbf-125">Accept</span></span>|<span data-ttu-id="f0bbf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f0bbf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0bbf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f0bbf-127">Request body</span></span>
<span data-ttu-id="f0bbf-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f0bbf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0bbf-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0bbf-129">Response</span></span>
<span data-ttu-id="f0bbf-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f0bbf-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f0bbf-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f0bbf-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f0bbf-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0bbf-132">Request</span></span>
<span data-ttu-id="f0bbf-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0bbf-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

### <a name="response"></a><span data-ttu-id="f0bbf-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0bbf-134">Response</span></span>
<span data-ttu-id="f0bbf-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f0bbf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





