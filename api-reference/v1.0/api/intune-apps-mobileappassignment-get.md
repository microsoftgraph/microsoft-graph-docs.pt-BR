---
title: Acessar mobileAppAssignment
description: Leia as propriedades e as relações do objeto mobileAppAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e214d8c3076121b7c4e053488755afd0ad9154cd
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30261478"
---
# <a name="get-mobileappassignment"></a><span data-ttu-id="6b295-103">Acessar mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="6b295-103">Get mobileAppAssignment</span></span>

> <span data-ttu-id="6b295-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6b295-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b295-105">Leia as propriedades e as relações do objeto [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6b295-105">Read properties and relationships of the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6b295-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6b295-106">Prerequisites</span></span>
<span data-ttu-id="6b295-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="6b295-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6b295-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6b295-109">Permission type</span></span>|<span data-ttu-id="6b295-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6b295-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b295-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6b295-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6b295-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6b295-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6b295-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6b295-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b295-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b295-114">Not supported.</span></span>|
|<span data-ttu-id="6b295-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b295-115">Application</span></span>|<span data-ttu-id="6b295-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b295-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b295-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6b295-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6b295-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6b295-118">Optional query parameters</span></span>
<span data-ttu-id="6b295-119">Este método dá suporte a [Parâmetros de consulta OData](https://docs.microsoft.com/en-us/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6b295-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6b295-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6b295-120">Request headers</span></span>
|<span data-ttu-id="6b295-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6b295-121">Header</span></span>|<span data-ttu-id="6b295-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6b295-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b295-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6b295-123">Authorization</span></span>|<span data-ttu-id="6b295-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6b295-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b295-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6b295-125">Accept</span></span>|<span data-ttu-id="6b295-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6b295-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b295-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6b295-127">Request body</span></span>
<span data-ttu-id="6b295-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6b295-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b295-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b295-129">Response</span></span>
<span data-ttu-id="6b295-130">Se tiver êxito, este método retornará o código de resposta `200 OK` e o objeto [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6b295-130">If successful, this method returns a `200 OK` response code and [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b295-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6b295-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b295-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6b295-132">Request</span></span>
<span data-ttu-id="6b295-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6b295-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

### <a name="response"></a><span data-ttu-id="6b295-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b295-134">Response</span></span>
<span data-ttu-id="6b295-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6b295-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



