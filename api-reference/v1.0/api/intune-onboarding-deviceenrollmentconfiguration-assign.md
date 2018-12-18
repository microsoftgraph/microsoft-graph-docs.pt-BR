---
title: atribuir ação
description: Ainda não documentado
author: tfitzmac
ms.openlocfilehash: 6812f3c1879c331cc27aeb25ea4516af080252b7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315299"
---
# <a name="assign-action"></a><span data-ttu-id="91803-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="91803-103">assign action</span></span>

> <span data-ttu-id="91803-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="91803-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="91803-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="91803-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="91803-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="91803-106">Prerequisites</span></span>
<span data-ttu-id="91803-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91803-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91803-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91803-109">Permission type</span></span>|<span data-ttu-id="91803-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="91803-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91803-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91803-111">Delegated (work or school account)</span></span>|<span data-ttu-id="91803-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91803-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="91803-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91803-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91803-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91803-114">Not supported.</span></span>|
|<span data-ttu-id="91803-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="91803-115">Application</span></span>|<span data-ttu-id="91803-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91803-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="91803-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91803-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="91803-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="91803-118">Request headers</span></span>
|<span data-ttu-id="91803-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="91803-119">Header</span></span>|<span data-ttu-id="91803-120">Valor</span><span class="sxs-lookup"><span data-stu-id="91803-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91803-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="91803-121">Authorization</span></span>|<span data-ttu-id="91803-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91803-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91803-123">Accept</span><span class="sxs-lookup"><span data-stu-id="91803-123">Accept</span></span>|<span data-ttu-id="91803-124">application/json</span><span class="sxs-lookup"><span data-stu-id="91803-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91803-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="91803-125">Request body</span></span>
<span data-ttu-id="91803-126">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="91803-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="91803-127">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="91803-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="91803-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="91803-128">Property</span></span>|<span data-ttu-id="91803-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="91803-129">Type</span></span>|<span data-ttu-id="91803-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="91803-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91803-131">enrollmentConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="91803-131">enrollmentConfigurationAssignments</span></span>|<span data-ttu-id="91803-132">Conjunto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="91803-132">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="91803-133">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="91803-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="91803-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="91803-134">Response</span></span>
<span data-ttu-id="91803-135">Se tiver êxito, esta ação retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="91803-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="91803-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="91803-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="91803-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91803-137">Request</span></span>
<span data-ttu-id="91803-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="91803-138">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="91803-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="91803-139">Response</span></span>
<span data-ttu-id="91803-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="91803-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



