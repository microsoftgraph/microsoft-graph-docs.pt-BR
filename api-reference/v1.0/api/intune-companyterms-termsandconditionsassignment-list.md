---
title: Listar termsAndConditionsAssignments
description: Listar propriedades e relações dos objetos termsAndConditionsAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0ae712e3fc2d4f4490652c3b74aa69e61df12f0d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825050"
---
# <a name="list-termsandconditionsassignments"></a><span data-ttu-id="c0c98-103">Listar termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="c0c98-103">List termsAndConditionsAssignments</span></span>

> <span data-ttu-id="c0c98-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c0c98-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c0c98-105">Listar propriedades e relações dos objetos [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).</span><span class="sxs-lookup"><span data-stu-id="c0c98-105">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c0c98-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c0c98-106">Prerequisites</span></span>
<span data-ttu-id="c0c98-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c0c98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0c98-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c0c98-109">Permission type</span></span>|<span data-ttu-id="c0c98-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c0c98-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0c98-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c0c98-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c0c98-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="c0c98-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="c0c98-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c0c98-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0c98-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0c98-114">Not supported.</span></span>|
|<span data-ttu-id="c0c98-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c0c98-115">Application</span></span>|<span data-ttu-id="c0c98-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c0c98-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0c98-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c0c98-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="c0c98-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c0c98-118">Request headers</span></span>
|<span data-ttu-id="c0c98-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c0c98-119">Header</span></span>|<span data-ttu-id="c0c98-120">Valor</span><span class="sxs-lookup"><span data-stu-id="c0c98-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0c98-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="c0c98-121">Authorization</span></span>|<span data-ttu-id="c0c98-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c0c98-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0c98-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c0c98-123">Accept</span></span>|<span data-ttu-id="c0c98-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c0c98-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0c98-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c0c98-125">Request body</span></span>
<span data-ttu-id="c0c98-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c0c98-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c0c98-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0c98-127">Response</span></span>
<span data-ttu-id="c0c98-128">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c0c98-128">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0c98-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c0c98-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="c0c98-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c0c98-130">Request</span></span>
<span data-ttu-id="c0c98-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c0c98-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

### <a name="response"></a><span data-ttu-id="c0c98-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="c0c98-132">Response</span></span>
<span data-ttu-id="c0c98-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c0c98-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



