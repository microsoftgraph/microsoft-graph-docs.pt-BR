---
title: atribuir ação
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f0576cefc39731aa0ca1097191704b6dc5d1c44b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876752"
---
# <a name="assign-action"></a><span data-ttu-id="80653-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="80653-103">assign action</span></span>

> <span data-ttu-id="80653-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="80653-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="80653-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="80653-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="80653-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="80653-106">Prerequisites</span></span>
<span data-ttu-id="80653-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80653-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80653-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="80653-109">Permission type</span></span>|<span data-ttu-id="80653-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="80653-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80653-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="80653-111">Delegated (work or school account)</span></span>|<span data-ttu-id="80653-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80653-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="80653-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="80653-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80653-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80653-114">Not supported.</span></span>|
|<span data-ttu-id="80653-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="80653-115">Application</span></span>|<span data-ttu-id="80653-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80653-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="80653-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="80653-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="80653-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="80653-118">Request headers</span></span>
|<span data-ttu-id="80653-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="80653-119">Header</span></span>|<span data-ttu-id="80653-120">Valor</span><span class="sxs-lookup"><span data-stu-id="80653-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80653-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="80653-121">Authorization</span></span>|<span data-ttu-id="80653-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="80653-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80653-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="80653-123">Accept</span></span>|<span data-ttu-id="80653-124">application/json</span><span class="sxs-lookup"><span data-stu-id="80653-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80653-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="80653-125">Request body</span></span>
<span data-ttu-id="80653-126">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="80653-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="80653-127">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="80653-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="80653-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80653-128">Property</span></span>|<span data-ttu-id="80653-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="80653-129">Type</span></span>|<span data-ttu-id="80653-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="80653-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80653-131">enrollmentConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="80653-131">enrollmentConfigurationAssignments</span></span>|<span data-ttu-id="80653-132">Conjunto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="80653-132">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="80653-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="80653-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="80653-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="80653-134">Response</span></span>
<span data-ttu-id="80653-135">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="80653-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="80653-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="80653-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="80653-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="80653-137">Request</span></span>
<span data-ttu-id="80653-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="80653-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assign

Content-type: application/json
Content-length: 304

{
  "enrollmentConfigurationAssignments": [
    {
      "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
      "id": "705b021c-021c-705b-1c02-5b701c025b70",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="80653-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="80653-139">Response</span></span>
<span data-ttu-id="80653-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="80653-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



