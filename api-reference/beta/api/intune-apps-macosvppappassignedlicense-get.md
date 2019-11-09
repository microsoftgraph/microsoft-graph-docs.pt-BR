---
title: Obter macOsVppAppAssignedLicense
description: Leia as propriedades e as relações do objeto macOsVppAppAssignedLicense.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: da552af03351fdf2195c78954bcb1e51f2135d69
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/09/2019
ms.locfileid: "38080172"
---
# <a name="get-macosvppappassignedlicense"></a><span data-ttu-id="81a03-103">Obter macOsVppAppAssignedLicense</span><span class="sxs-lookup"><span data-stu-id="81a03-103">Get macOsVppAppAssignedLicense</span></span>

> <span data-ttu-id="81a03-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="81a03-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81a03-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="81a03-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81a03-106">Leia as propriedades e as relações do objeto [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) .</span><span class="sxs-lookup"><span data-stu-id="81a03-106">Read properties and relationships of the [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="81a03-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="81a03-107">Prerequisites</span></span>
<span data-ttu-id="81a03-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="81a03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81a03-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="81a03-110">Permission type</span></span>|<span data-ttu-id="81a03-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="81a03-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81a03-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="81a03-112">Delegated (work or school account)</span></span>|<span data-ttu-id="81a03-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="81a03-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="81a03-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="81a03-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81a03-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="81a03-115">Not supported.</span></span>|
|<span data-ttu-id="81a03-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="81a03-116">Application</span></span>|<span data-ttu-id="81a03-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="81a03-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="81a03-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="81a03-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses/{macOsVppAppAssignedLicenseId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="81a03-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="81a03-119">Optional query parameters</span></span>
<span data-ttu-id="81a03-120">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="81a03-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="81a03-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="81a03-121">Request headers</span></span>
|<span data-ttu-id="81a03-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="81a03-122">Header</span></span>|<span data-ttu-id="81a03-123">Valor</span><span class="sxs-lookup"><span data-stu-id="81a03-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81a03-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="81a03-124">Authorization</span></span>|<span data-ttu-id="81a03-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="81a03-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81a03-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="81a03-126">Accept</span></span>|<span data-ttu-id="81a03-127">application/json</span><span class="sxs-lookup"><span data-stu-id="81a03-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81a03-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="81a03-128">Request body</span></span>
<span data-ttu-id="81a03-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="81a03-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81a03-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="81a03-130">Response</span></span>
<span data-ttu-id="81a03-131">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="81a03-131">If successful, this method returns a `200 OK` response code and [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="81a03-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="81a03-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="81a03-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="81a03-133">Request</span></span>
<span data-ttu-id="81a03-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="81a03-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses/{macOsVppAppAssignedLicenseId}
```

### <a name="response"></a><span data-ttu-id="81a03-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="81a03-135">Response</span></span>
<span data-ttu-id="81a03-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="81a03-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 316

{
  "value": {
    "@odata.type": "#microsoft.graph.macOsVppAppAssignedLicense",
    "id": "a1204d8e-4d8e-a120-8e4d-20a18e4d20a1",
    "userEmailAddress": "User Email Address value",
    "userId": "User Id value",
    "userName": "User Name value",
    "userPrincipalName": "User Principal Name value"
  }
}
```






