---
title: Listar deviceCompliancePolicyAssignments
description: Listar propriedades e relações dos objetosdeviceCompliancePolicyAssignment.
ms.openlocfilehash: 5ef75a78265324493fc86fdac198b49c2d616edc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039081"
---
# <a name="list-devicecompliancepolicyassignments"></a><span data-ttu-id="28413-103">Listar deviceCompliancePolicyAssignments</span><span class="sxs-lookup"><span data-stu-id="28413-103">List deviceCompliancePolicyAssignments</span></span>

> <span data-ttu-id="28413-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="28413-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="28413-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="28413-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="28413-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="28413-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="28413-107">Listar propriedades e relações dos objetos[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md).</span><span class="sxs-lookup"><span data-stu-id="28413-107">List properties and relationships of the [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="28413-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="28413-108">Prerequisites</span></span>
<span data-ttu-id="28413-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="28413-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28413-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="28413-111">Permission type</span></span>|<span data-ttu-id="28413-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="28413-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="28413-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="28413-113">Delegated (work or school account)</span></span>|<span data-ttu-id="28413-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="28413-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="28413-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="28413-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="28413-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28413-116">Not supported.</span></span>|
|<span data-ttu-id="28413-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="28413-117">Application</span></span>|<span data-ttu-id="28413-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="28413-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="28413-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="28413-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="28413-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="28413-120">Request headers</span></span>
|<span data-ttu-id="28413-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="28413-121">Header</span></span>|<span data-ttu-id="28413-122">Valor</span><span class="sxs-lookup"><span data-stu-id="28413-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="28413-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="28413-123">Authorization</span></span>|<span data-ttu-id="28413-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="28413-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="28413-125">Accept</span><span class="sxs-lookup"><span data-stu-id="28413-125">Accept</span></span>|<span data-ttu-id="28413-126">application/json</span><span class="sxs-lookup"><span data-stu-id="28413-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="28413-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="28413-127">Request body</span></span>
<span data-ttu-id="28413-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="28413-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="28413-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="28413-129">Response</span></span>
<span data-ttu-id="28413-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="28413-130">If successful, this method returns a `200 OK` response code and a collection of [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28413-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="28413-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="28413-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="28413-132">Request</span></span>
<span data-ttu-id="28413-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="28413-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assignments
```

### <a name="response"></a><span data-ttu-id="28413-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="28413-134">Response</span></span>
<span data-ttu-id="28413-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="28413-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 274

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCompliancePolicyAssignment",
      "id": "92dc3fef-3fef-92dc-ef3f-dc92ef3fdc92",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```





