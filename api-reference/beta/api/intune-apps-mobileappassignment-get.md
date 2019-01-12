---
title: Acessar mobileAppAssignment
description: Leia as propriedades e as relações do objeto mobileAppAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6d240b0d597e51df729b6bfce8d8c87e4dbfa252
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984966"
---
# <a name="get-mobileappassignment"></a><span data-ttu-id="d9a39-103">Acessar mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="d9a39-103">Get mobileAppAssignment</span></span>

> <span data-ttu-id="d9a39-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d9a39-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d9a39-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d9a39-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d9a39-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d9a39-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d9a39-107">Leia as propriedades e as relações do objeto [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="d9a39-107">Read properties and relationships of the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d9a39-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d9a39-108">Prerequisites</span></span>
<span data-ttu-id="d9a39-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9a39-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9a39-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9a39-111">Permission type</span></span>|<span data-ttu-id="d9a39-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d9a39-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9a39-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9a39-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d9a39-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d9a39-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d9a39-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9a39-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9a39-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9a39-116">Not supported.</span></span>|
|<span data-ttu-id="d9a39-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9a39-117">Application</span></span>|<span data-ttu-id="d9a39-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9a39-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9a39-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9a39-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d9a39-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d9a39-120">Optional query parameters</span></span>
<span data-ttu-id="d9a39-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d9a39-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d9a39-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9a39-122">Request headers</span></span>
|<span data-ttu-id="d9a39-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d9a39-123">Header</span></span>|<span data-ttu-id="d9a39-124">Valor</span><span class="sxs-lookup"><span data-stu-id="d9a39-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9a39-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9a39-125">Authorization</span></span>|<span data-ttu-id="d9a39-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9a39-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9a39-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d9a39-127">Accept</span></span>|<span data-ttu-id="d9a39-128">application/json</span><span class="sxs-lookup"><span data-stu-id="d9a39-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9a39-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9a39-129">Request body</span></span>
<span data-ttu-id="d9a39-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d9a39-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9a39-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9a39-131">Response</span></span>
<span data-ttu-id="d9a39-132">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d9a39-132">If successful, this method returns a `200 OK` response code and [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9a39-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d9a39-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="d9a39-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9a39-134">Request</span></span>
<span data-ttu-id="d9a39-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9a39-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

### <a name="response"></a><span data-ttu-id="d9a39-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9a39-136">Response</span></span>
<span data-ttu-id="d9a39-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d9a39-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 359

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppAssignment",
    "id": "591620b7-20b7-5916-b720-1659b7201659",
    "intent": "required",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    },
    "settings": {
      "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
    }
  }
}
```





