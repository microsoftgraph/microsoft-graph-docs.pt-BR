---
title: Obter iosVppAppAssignedLicense
description: Leia as propriedades e os relacionamentos do objeto iosVppAppAssignedLicense.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2d45eb37ea2471c83743dbb6b5bfe497d9c89537
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808929"
---
# <a name="get-iosvppappassignedlicense"></a><span data-ttu-id="da109-103">Obter iosVppAppAssignedLicense</span><span class="sxs-lookup"><span data-stu-id="da109-103">Get iosVppAppAssignedLicense</span></span>

> <span data-ttu-id="da109-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="da109-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="da109-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="da109-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="da109-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="da109-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="da109-107">Leia as propriedades e os relacionamentos do objeto [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="da109-107">Read properties and relationships of the [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="da109-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="da109-108">Prerequisites</span></span>
<span data-ttu-id="da109-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da109-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da109-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="da109-111">Permission type</span></span>|<span data-ttu-id="da109-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="da109-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da109-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="da109-113">Delegated (work or school account)</span></span>|<span data-ttu-id="da109-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="da109-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="da109-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="da109-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da109-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da109-116">Not supported.</span></span>|
|<span data-ttu-id="da109-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="da109-117">Application</span></span>|<span data-ttu-id="da109-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="da109-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="da109-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="da109-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="da109-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="da109-120">Optional query parameters</span></span>
<span data-ttu-id="da109-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="da109-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="da109-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="da109-122">Request headers</span></span>
|<span data-ttu-id="da109-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="da109-123">Header</span></span>|<span data-ttu-id="da109-124">Valor</span><span class="sxs-lookup"><span data-stu-id="da109-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da109-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="da109-125">Authorization</span></span>|<span data-ttu-id="da109-126">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="da109-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da109-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="da109-127">Accept</span></span>|<span data-ttu-id="da109-128">application/json</span><span class="sxs-lookup"><span data-stu-id="da109-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da109-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="da109-129">Request body</span></span>
<span data-ttu-id="da109-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="da109-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da109-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="da109-131">Response</span></span>
<span data-ttu-id="da109-132">Se tiver êxito, este método retornará um `200 OK` objeto response de código e [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="da109-132">If successful, this method returns a `200 OK` response code and [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da109-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="da109-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="da109-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="da109-134">Request</span></span>
<span data-ttu-id="da109-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="da109-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses/{iosVppAppAssignedLicenseId}
```

### <a name="response"></a><span data-ttu-id="da109-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="da109-136">Response</span></span>
<span data-ttu-id="da109-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="da109-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 314

{
  "value": {
    "@odata.type": "#microsoft.graph.iosVppAppAssignedLicense",
    "id": "090a8d2e-8d2e-090a-2e8d-0a092e8d0a09",
    "userEmailAddress": "User Email Address value",
    "userId": "User Id value",
    "userName": "User Name value",
    "userPrincipalName": "User Principal Name value"
  }
}
```





