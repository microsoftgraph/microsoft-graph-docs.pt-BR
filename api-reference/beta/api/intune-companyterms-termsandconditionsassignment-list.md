---
title: Listar termsAndConditionsAssignments
description: Listar propriedades e relações dos objetos termsAndConditionsAssignment.
ms.openlocfilehash: 79a8533a556cfc78944948403f2cfa533284c748
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040001"
---
# <a name="list-termsandconditionsassignments"></a><span data-ttu-id="a3fee-103">Listar termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="a3fee-103">List termsAndConditionsAssignments</span></span>

> <span data-ttu-id="a3fee-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a3fee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a3fee-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a3fee-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a3fee-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a3fee-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a3fee-107">Listar propriedades e relações dos objetos [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="a3fee-107">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a3fee-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a3fee-108">Prerequisites</span></span>
<span data-ttu-id="a3fee-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3fee-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3fee-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a3fee-111">Permission type</span></span>|<span data-ttu-id="a3fee-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a3fee-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3fee-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a3fee-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a3fee-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="a3fee-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="a3fee-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a3fee-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3fee-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3fee-116">Not supported.</span></span>|
|<span data-ttu-id="a3fee-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a3fee-117">Application</span></span>|<span data-ttu-id="a3fee-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3fee-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3fee-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a3fee-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="a3fee-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a3fee-120">Request headers</span></span>
|<span data-ttu-id="a3fee-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a3fee-121">Header</span></span>|<span data-ttu-id="a3fee-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a3fee-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3fee-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a3fee-123">Authorization</span></span>|<span data-ttu-id="a3fee-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a3fee-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3fee-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a3fee-125">Accept</span></span>|<span data-ttu-id="a3fee-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a3fee-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3fee-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a3fee-127">Request body</span></span>
<span data-ttu-id="a3fee-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a3fee-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3fee-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3fee-129">Response</span></span>
<span data-ttu-id="a3fee-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a3fee-130">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3fee-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a3fee-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="a3fee-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a3fee-132">Request</span></span>
<span data-ttu-id="a3fee-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a3fee-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

### <a name="response"></a><span data-ttu-id="a3fee-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3fee-134">Response</span></span>
<span data-ttu-id="a3fee-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a3fee-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 270

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
      "id": "64c1a196-a196-64c1-96a1-c16496a1c164",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```





