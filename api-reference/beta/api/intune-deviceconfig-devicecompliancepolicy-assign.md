---
title: atribuir ação
description: Ainda não documentado
ms.openlocfilehash: 9cca8b47cd857bce017858d24375b77ea822980d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034251"
---
# <a name="assign-action"></a><span data-ttu-id="d10a6-103">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="d10a6-103">assign action</span></span>

> <span data-ttu-id="d10a6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d10a6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d10a6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d10a6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d10a6-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d10a6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d10a6-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d10a6-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d10a6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d10a6-108">Prerequisites</span></span>
<span data-ttu-id="d10a6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d10a6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d10a6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d10a6-111">Permission type</span></span>|<span data-ttu-id="d10a6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d10a6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d10a6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d10a6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d10a6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d10a6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d10a6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d10a6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d10a6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d10a6-116">Not supported.</span></span>|
|<span data-ttu-id="d10a6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d10a6-117">Application</span></span>|<span data-ttu-id="d10a6-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d10a6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d10a6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d10a6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="d10a6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d10a6-120">Request headers</span></span>
|<span data-ttu-id="d10a6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d10a6-121">Header</span></span>|<span data-ttu-id="d10a6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d10a6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d10a6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d10a6-123">Authorization</span></span>|<span data-ttu-id="d10a6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d10a6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d10a6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d10a6-125">Accept</span></span>|<span data-ttu-id="d10a6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d10a6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d10a6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d10a6-127">Request body</span></span>
<span data-ttu-id="d10a6-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="d10a6-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="d10a6-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="d10a6-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="d10a6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d10a6-130">Property</span></span>|<span data-ttu-id="d10a6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="d10a6-131">Type</span></span>|<span data-ttu-id="d10a6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="d10a6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d10a6-133">assignments</span><span class="sxs-lookup"><span data-stu-id="d10a6-133">assignments</span></span>|<span data-ttu-id="d10a6-134">Coleção [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d10a6-134">[deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection</span></span>|<span data-ttu-id="d10a6-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d10a6-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="d10a6-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d10a6-136">Response</span></span>
<span data-ttu-id="d10a6-137">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d10a6-137">If successful, this action returns a `200 OK` response code and a [deviceCompliancePolicyAssignment](../resources/intune-deviceconfig-devicecompliancepolicyassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d10a6-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d10a6-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="d10a6-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d10a6-139">Request</span></span>
<span data-ttu-id="d10a6-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d10a6-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/assign

Content-type: application/json
Content-length: 280

{
  "assignments": [
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

### <a name="response"></a><span data-ttu-id="d10a6-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="d10a6-141">Response</span></span>
<span data-ttu-id="d10a6-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d10a6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





