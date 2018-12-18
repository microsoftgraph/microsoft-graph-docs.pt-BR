---
title: Listar enrollmentConfigurationAssignments
description: Listar propriedades e relações de objetos de enrollmentConfigurationAssignment.
author: tfitzmac
ms.openlocfilehash: 0aad76f06d9694c4abaedcd728f3df10a817865c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351776"
---
# <a name="list-enrollmentconfigurationassignments"></a><span data-ttu-id="8298f-103">Listar enrollmentConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="8298f-103">List enrollmentConfigurationAssignments</span></span>

> <span data-ttu-id="8298f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8298f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8298f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8298f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8298f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8298f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8298f-107">Listar propriedades e relações de objetos de [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="8298f-107">List properties and relationships of the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8298f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8298f-108">Prerequisites</span></span>
<span data-ttu-id="8298f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8298f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8298f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8298f-111">Permission type</span></span>|<span data-ttu-id="8298f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8298f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8298f-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8298f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8298f-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="8298f-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="8298f-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8298f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8298f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8298f-116">Not supported.</span></span>|
|<span data-ttu-id="8298f-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8298f-117">Application</span></span>|<span data-ttu-id="8298f-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8298f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8298f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8298f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="8298f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8298f-120">Request headers</span></span>
|<span data-ttu-id="8298f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8298f-121">Header</span></span>|<span data-ttu-id="8298f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8298f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8298f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8298f-123">Authorization</span></span>|<span data-ttu-id="8298f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8298f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8298f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8298f-125">Accept</span></span>|<span data-ttu-id="8298f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8298f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8298f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8298f-127">Request body</span></span>
<span data-ttu-id="8298f-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8298f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8298f-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8298f-129">Response</span></span>
<span data-ttu-id="8298f-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8298f-130">If successful, this method returns a `200 OK` response code and a collection of [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8298f-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8298f-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="8298f-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8298f-132">Request</span></span>
<span data-ttu-id="8298f-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8298f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="8298f-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8298f-134">Response</span></span>
<span data-ttu-id="8298f-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8298f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "value": [
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





