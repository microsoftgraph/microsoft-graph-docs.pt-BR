---
title: Obter termsAndConditionsAssignment
description: Ler propriedades e relações do objeto termsAndConditionsAssignment.
author: tfitzmac
ms.openlocfilehash: eb0f56703e50a48966dc2a8c27aa6a66e5fbdb6b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319436"
---
# <a name="get-termsandconditionsassignment"></a><span data-ttu-id="02df6-103">Obter termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="02df6-103">Get termsAndConditionsAssignment</span></span>

> <span data-ttu-id="02df6-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="02df6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="02df6-105">Ler propriedades e relações do objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="02df6-105">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="02df6-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="02df6-106">Prerequisites</span></span>
<span data-ttu-id="02df6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="02df6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02df6-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="02df6-109">Permission type</span></span>|<span data-ttu-id="02df6-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="02df6-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02df6-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="02df6-111">Delegated (work or school account)</span></span>|<span data-ttu-id="02df6-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="02df6-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="02df6-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="02df6-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02df6-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02df6-114">Not supported.</span></span>|
|<span data-ttu-id="02df6-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="02df6-115">Application</span></span>|<span data-ttu-id="02df6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="02df6-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="02df6-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="02df6-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="02df6-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="02df6-118">Optional query parameters</span></span>
<span data-ttu-id="02df6-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="02df6-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="02df6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="02df6-120">Request headers</span></span>
|<span data-ttu-id="02df6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="02df6-121">Header</span></span>|<span data-ttu-id="02df6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="02df6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02df6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="02df6-123">Authorization</span></span>|<span data-ttu-id="02df6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="02df6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02df6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="02df6-125">Accept</span></span>|<span data-ttu-id="02df6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="02df6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02df6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="02df6-127">Request body</span></span>
<span data-ttu-id="02df6-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="02df6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02df6-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="02df6-129">Response</span></span>
<span data-ttu-id="02df6-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="02df6-130">If successful, this method returns a `200 OK` response code and [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02df6-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="02df6-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="02df6-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="02df6-132">Request</span></span>
<span data-ttu-id="02df6-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="02df6-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments/{termsAndConditionsAssignmentId}
```

### <a name="response"></a><span data-ttu-id="02df6-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="02df6-134">Response</span></span>
<span data-ttu-id="02df6-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="02df6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 246

{
  "value": {
    "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
    "id": "64c1a196-a196-64c1-96a1-c16496a1c164",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```



